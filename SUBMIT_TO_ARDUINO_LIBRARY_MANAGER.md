# Submit To Arduino Library Manager

File nay la checklist ngan gon de dua `OhStemRobotics` vao Arduino Library Manager.

## 1. Push code len GitHub

Chay cac lenh sau trong repo:

```powershell
git add .
git commit -m "Restructure library for Arduino Library Manager"
git push origin main
```

Neu branch chinh cua anh khong phai `main` thi doi lai ten branch cho dung.

## 2. Tao tag va GitHub Release

Arduino Library Manager chi index cac ban phat hanh co tag Semantic Versioning.

Vi du release dau tien:

```powershell
git tag 0.2.0
git push origin 0.2.0
```

Sau do vao GitHub:

1. Mo repo `truongphat230799/ohstem-orc-hub-robotics`
2. Vao `Releases`
3. Chon `Draft a new release`
4. Chon tag `0.2.0`
5. Dat title: `OhStemRobotics 0.2.0`

Noi dung release co the dung mau nay:

```text
OhStemRobotics 0.2.0

- Restructure repository to standard Arduino library layout
- Keep library source in root-level src/
- Provide examples in root-level examples/
- Add library metadata for Arduino IDE and Library Manager
- Add keywords.txt for Arduino IDE highlighting
```

## 3. Tao PR dang ky vao Arduino Library Manager

Arduino khong lay library moi tu dong. Anh can tao pull request vao:

`https://github.com/arduino/library-registry`

Tao file moi trong PR:

`repositories.txt`

va them dong nay:

```text
https://github.com/truongphat230799/ohstem-orc-hub-robotics.git
```

Neu repo `repositories.txt` da ton tai nhieu dong, chi can them them 1 dong URL ben tren.

## 4. Noi dung PR mau

Title goi y:

```text
Add OhStemRobotics library
```

Body goi y:

```text
This PR adds the OhStemRobotics library to Arduino Library Manager.

Repository:
https://github.com/truongphat230799/ohstem-orc-hub-robotics

Library name:
OhStemRobotics

Current release:
0.2.0

The repository has been structured as a standard Arduino library and includes:
- src/
- examples/
- library.properties
- keywords.txt

Thank you.
```

## 5. Sau khi PR duoc merge

Sau khi PR trong `arduino/library-registry` duoc merge, Arduino se mat mot khoang thoi gian de index.

Luc do nguoi dung co the tim thu vien trong:

`Arduino IDE > Library Manager`

Tu khoa tim kiem:

`OhStemRobotics`

## 6. Luu y cho cac release sau

Moi lan cap nhat thu vien:

1. Sua `version` trong `library.properties`
2. Tao tag moi theo semver, vi du `0.2.1`
3. Tao GitHub Release cho tag do

Lenh mau:

```powershell
git add .
git commit -m "Release 0.2.1"
git push origin main
git tag 0.2.1
git push origin 0.2.1
```
