### Menambahkan "Open with code" di Windows Explorer dengan menambahkan registry
1. cari folder program vscode setelah mendapatkannya copy path "code.exe" "C:\Program Files\Microsoft VS Code\Code.exe"
1. buka notepad ketik kode berikut 

; Klik kanan pada File
[HKEY_CLASSES_ROOT\*\shell\VSCode]
@="Open with Code"
"Icon"="C:\\Program Files\\Microsoft VS Code\\Code.exe"

[HKEY_CLASSES_ROOT\*\shell\VSCode\command]
@="\"C:\\Program Files\\Microsoft VS Code\\Code.exe\" \"%1\""

; Klik kanan pada Folder
[HKEY_CLASSES_ROOT\Directory\shell\VSCode]
@="Open with Code"
"Icon"="C:\\Program Files\\Microsoft VS Code\\Code.exe"

[HKEY_CLASSES_ROOT\Directory\shell\VSCode\command]
@="\"C:\\Program Files\\Microsoft VS Code\\Code.exe\" \"%1\""

; Klik kanan pada Area Kosong di Dalam Folder
[HKEY_CLASSES_ROOT\Directory\Background\shell\VSCode]
@="Open with Code"
"Icon"="C:\\Program Files\\Microsoft VS Code\\Code.exe"

[HKEY_CLASSES_ROOT\Directory\Background\shell\VSCode\command]
@="\"C:\\Program Files\\Microsoft VS Code\\Code.exe\" \"%V\""

1. sesuaikan file path code.exe
1. simpan dan ubah ekstensi menjadi .reg
1. uban menjadi all file dan save
1. double click pada file yang sudah di simpan