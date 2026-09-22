# C++ Setup Guide — VS Code + MSYS2 + PowerShell

This guide is for Windows students using Visual Studio Code.

## 1. Install Visual Studio Code

Install VS Code, then install the extension:

```text
C/C++ — Microsoft
```

The extension is not the compiler. You still need `g++`.

## 2. Install MSYS2

Install MSYS2.

Open the **MSYS2 UCRT64** terminal and run:

```bash
pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain
```

## 3. Add g++ to Windows PATH

The compiler is usually located at:

```text
C:\msys64\ucrt64\bin
```

Test temporarily in PowerShell:

```powershell
$env:Path += ";C:\msys64\ucrt64\bin"
g++ --version
```

If it works, add that folder permanently to your Windows User PATH.

Restart VS Code after updating PATH.

## 4. Verify

Open PowerShell:

```powershell
g++ --version
where.exe g++
```

Expected compiler location:

```text
C:\msys64\ucrt64\bin\g++.exe
```

## 5. Create a Test File

Create:

```text
exercise.cpp
```

Content:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello C++!" << endl;
    return 0;
}
```

## 6. Compile

```powershell
g++ exercise.cpp -o exercise
```

## 7. Run

```powershell
.\exercise.exe
```

Expected output:

```text
Hello C++!
```

## Common Error

If you see:

```text
g++ : The term 'g++' is not recognized...
```

Check:

1. MSYS2 toolchain is installed.
2. `C:\msys64\ucrt64\bin` exists.
3. The path is in Windows PATH.
4. VS Code was restarted.
5. `g++ --version` works in PowerShell.

If the error continues, create a GitHub Issue using the class troubleshooting guide.
