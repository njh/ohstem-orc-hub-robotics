# OhStemRobotics

Thu vien robotics cho Arduino IDE va PlatformIO, duoc to chuc theo dung cau truc Arduino library de co the publish len GitHub va dang ky voi Arduino Library Manager.

## Cau truc repo

- `src/`: ma nguon thu vien
- `examples/`: cac sketch mau mo truc tiep trong Arduino IDE
- `library.properties`: metadata bat buoc de Arduino IDE nhan dien thu vien
- `keywords.txt`: tu khoa highlight trong Arduino IDE

## Tinh nang chinh

- `MotorDriverV1`, `MotorDriverV2`
- `DCMotor`, `DCMotor2Pin`, `DCMotor3Pin`
- `RobotServo`
- `LineSensor2P`, `LineSensor3P`, `LineSensorI2C`
- `DriveBase`
- `Gamepad`, `PS4GamepadReceiver`
- `PIDController`
- `MPU6050Sensor`, `MPU9250Sensor`
- `AngleSensor`

## Vi du trong Arduino IDE

Sau khi cai thu vien, cac bai mau se hien trong:

`File > Examples > OhStemRobotics`

Repo hien dang gom:

- `BasicDrive`
- `LineFollower`
- `PS4Teleop`
- `Bai_01_Robot_di_chuyen`
- `Bai_02_Robot_ne_vat_can`
- `Bai_03_Robot_do_duong`
- `Bai_04_Dieu_khien_robot_tu_xa`
- `Bai_05_Dieu_khien_robot_gap_tha_vat`
- `Bai_06_Co_cau_truyen_dong`
- `Bai_07_Hoan_thien_robot_thi_dau`
- `Bai_01_Robot_4_banh_di_chuyen`
- `Bai_02_Robot_4_banh_ne_vat_can`
- `Bai_03_Robot_4_banh_do_duong`
- `Bai_04_Robot_4_banh_tu_xa`
- `Bai_07_Robot_4_banh_thi_dau`

## Dang ky de tim thay tren Arduino IDE

Chi dung cau truc dung chua du de thu vien tu dong xuat hien trong Arduino IDE. De co mat trong Library Manager, can them cac buoc sau:

1. Day repo len GitHub o trang public.
2. Tao release tag theo Semantic Versioning, vi du `0.2.0`.
3. Tao pull request toi repo `arduino/library-registry` de dang ky thu vien.
4. Sau khi duoc duyet, cho he thong Arduino index ban release moi.

Huong dan submit chi tiet da duoc dat trong [SUBMIT_TO_ARDUINO_LIBRARY_MANAGER.md](d:/OhStem/ohstem-orc-hub-robotics/SUBMIT_TO_ARDUINO_LIBRARY_MANAGER.md).

## Luu y tuong thich

- Thu vien dung cau truc Arduino library o root repo, khong long them mot thu muc thu vien khac ben trong.
- `library.properties` dang tro ve dung URL GitHub cua repo.
- Neu phan cung cua anh khac bo kit mac dinh, chi can sua thong so o dau cac file `.ino`.
