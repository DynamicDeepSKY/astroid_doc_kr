.. _recovery:

복구 안내
====================

복구 과정을 시작하기 전에 라이선스와 교정 파일을 백업해야 합니다.

1. 라이선스 파일 다운로드

.. figure:: /images/license_download.png
   :width: 400
   :alt: 라이선스 다운로드
   :align: center
   
2. 렌즈 교정 파일 다운로드

.. figure:: /images/calibration_download.png
   :width: 400
   :alt: 교정 다운로드
   :align: center
   
장치가 부팅되지 않아 이 파일들을 다운로드할 수 없는 경우, info@dynamicdeepsky.com 으로 연락해 주십시오. 가능한 한 빨리 해당 파일들을 보내드리겠습니다.
   
장치를 공장 초기 설정으로 복구하려면 다음 단계를 따르십시오.

1. Dynamicdeepsky.com의 지원 페이지에서 Astroid OS 이미지를 다운로드합니다.
2. https://www.raspberrypi.org/software/ 에서 Raspberry Pi Imager를 다운로드합니다.
3. Astroid에서 OS SD 카드를 분리하여 SD 카드 USB 어댑터나 내장 SD 카드 리더기를 통해 컴퓨터에 연결합니다.
4. 다운로드한 이미지로 SD 카드를 굽습니다.
5. SD 카드를 다시 Astroid에 넣고 전원을 연결합니다.
6. WIFI 목록에 "RPiHotspot"이 보일 때까지 5~10분 정도 기다립니다.

.. admonition:: 중요

    "RPiHotspot"이 보이기 전에 전원을 차단하면 3단계부터 다시 시작해야 합니다.
    

7. RPiHotspot에 연결하고 웹 브라우저에 다음 주소를 입력하여 시리얼 번호를 설정합니다:  

**http://10.10.10.10/setserial/YOUR_SERIALNUMBER**

예를 들어, 시리얼 번호가 1030001이라면 다음 명령을 사용합니다.

http://10.10.10.10/setserial/1030001

.. figure:: /images/set_serial.png
   :width: 400
   :alt: 시리얼 설정
   :align: center
   
시리얼 번호를 입력하면 장치의 WIFI ID가 DDS_DIRECT_1030001으로 변경됩니다.

8. 이제 라이선스와 시리얼을 설정해야 합니다. "System Setting" -> "License Management" 아래에 있는 "License Code File" 버튼을 클릭하고, 초기화 전에 다운로드한 파일을 선택합니다.

.. figure:: /images/license_upload.png
   :width: 400
   :alt: 라이선스 업로드
   :align: center

9. "System Setting" -> "Calibration" 아래의 "Load Calibration" 버튼을 클릭하고, 초기화 전에 다운로드한 파일을 선택합니다.

.. figure:: /images/calibration_upload.png
   :width: 400
   :alt: 교정 업로드
   :align: center
   
10. ShowInfo 창에서 시스템 버전을 확인하고, 구버전이라면 업데이트를 실행합니다. 자세한 내용은 :ref:`System Update <systemupdate>` 를 참조하십시오.

