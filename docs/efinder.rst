.. _efinder:

eFinder
=======

하단 아이콘 바의 눈 버튼 |liveps| 을 클릭하면 Astroid의 작동 모드가 eFinder로 전환되고 실시간 하늘 인식이 활성화됩니다. eFinder를 사용하기 전에 하늘이 인식되었는지 확인하십시오. 하늘이 인식되면 상태 바의 빨간 눈 아이콘 |eye_red| 이 녹색 눈 |eye_green| 으로 바뀝니다. 

.. |liveps| image:: /images/liveps.png
                :scale: 30 %

.. |eye_green| image:: /images/eye_green.png
                :scale: 30 %
                
.. |eye_red| image:: /images/eye_red.png
                :scale: 30 %
                
.. admonition:: 중요

    하늘 인식 모드는 제공된 5mm 렌즈에서만 작동한다는 점에 유의하세요. 다른 렌즈를 장착하여 Astroid를 카메라로 사용할 수는 있지만 하늘 인식은 작동하지 않습니다.
    
Sky Recognition
------------------------------------------------

하늘 인식이 활성화되면 Astroid가 하늘을 인식하려고 시도하지만 경우에 따라 실패할 수 있습니다. 5초 이내에 하늘 인식 상태 아이콘이 녹색으로 바뀌지 않는다면 다음을 시도해 보세요.

* 렌즈 초점이 맞는지 확인하세요. 초점이 흐리면 Astroid가 별을 잘 인식하지 못합니다.
* 이미지에 충분한 별이 있는지 확인하세요.
* 게인/노출을 약간 높이거나 낮추어 보세요. 이미지가 너무 밝거나 어둡지 않아야 합니다. 노출을 높이면 반응 속도가 느려집니다.
* 카메라를 구름, 달, 건물이 없는 방향으로 향하게 하세요. 보이는 장애물이 많으면 하늘 인식에 더 많은 시간이 걸립니다. 일단 인식되면 천천히 원하는 방향으로 카메라를 이동합니다.

Light Pollution
---------------------------------------------------

하늘 인식 성능에 영향을 미치는 주요 요인 중 하나는 하늘 상태입니다. 최적의 하늘 상태는 달빛이 없는 Bortle 6 이하의 매우 어두운 하늘입니다. Bortle은 야간 하늘의 빛 공해 정도를 추정하는 척도입니다. 다음 사이트에서 해당 위치의 Bortle 단계를 쉽게 확인할 수 있습니다.

https://www.lightpollutionmap.info/

다음 예시는 브리즈번 시내 주변의 세 장소에 대한 Bortle 단계를 보여줍니다.

.. figure:: /images/bortle.png
   :width: 600
   :alt: Bortle
   :align: center

작동할 수도 있지만 Bortle 6 이상 고도한 빛 공해 지역에서는 하늘 인식 성능을 보장하지 않습니다. Bortle 등급에 대한 자세한 내용은 다음 표를 참조하세요.


.. list-table:: Bortle 등급
   :align: center
   :widths: 50 25
   :header-rows: 1   

   * - 하늘 상태
     - Bortle 등급
   * - 탁월한 암흑 하늘
     - 1
   * - 평균 암흑 하늘
     - 2
   * - 시골 하늘
     - 3
   * - 시골/교외 전환
     - 4     
   * - 교외
     - 5
   * - 밝은 교외
     - 6
   * - 교외/도시 전환
     - 7
   * - 도시 하늘
     - 8     
   * - 도심 하늘
     - 9        

    
Sky Recognition with Moon Light or Light Pollution
---------------------------------------------------

달빛이나 빛 공해 하에서는 Bortle 6 이하, 달빛 없는 상태에서 사용하는 것이 권장되지만, 그렇지 않은 환경에서도 제한된 속도와 정확도로 eFinder를 작동시키는 방법이 있습니다.

하늘 인식의 기본 설정은 달빛 없는 Bortle 5에 최적화된 노출 0.3초, 게인 140입니다. 짧은 노출 시간은 반응 속도를 높여주지만 높은 게인 설정이 필요하며, 이는 빛 공해 및 달빛 조건에서 노이즈가 많은 이미지를 초래합니다. 노이즈가 많은 이미지는 하늘 인식 성능을 떨어뜨립니다.   

간단한 해결책은 노출을 늘리고 게인을 낮춰 반응 속도를 타협하는 것입니다. 다음 예시는 노출 및 게인 설정이 달빛 조건에서 노이즈를 줄이는 방법을 보여줍니다.  

.. figure:: /images/light_condition_low_exposure.png
   :width: 400
   :alt: Low exposure
   :align: center   
   
.. figure:: /images/light_condition_max_exposure.png
   :width: 400
   :alt: Max exposure
   :align: center


Automatic DSO search |autodso_search|
----------------------------------------------------

자동 DSO 검색은 아무런 준비 없이 자유롭게 하늘을 탐험하고 싶을 때 매우 유용합니다. 이 기능을 활성화하면 현재 주요 망원경 시야에 가장 가까운 DSO를 자동으로 찾아 화면에 모양과 ID를 표시합니다.

.. |autodso_search| image:: /images/autodso_search.png
                :scale: 40 %

기본적으로 이 기능은 NGC에 있는 천체를 표시하지만 "Astro Tools Menu" -> "Search Setting" 에서 다른 카탈로그를 선택할 수 있습니다. 또한, 접안렌즈의 시야에 따라 너무 작거나 너무 큰 별을 찾고 싶지 않을 수 있습니다. Min 및 Max 크기 옵션을 조정하세요.

이 옵션을 켠 후 화면에 아무 것도 보이지 않으면, 약간 확대하고 하늘의 다른 부분을 이동해 보세요.

Geolocation and Time
------------------------------------------------

시스템 시간은 기기의 시간에 따라 자동으로 업데이트되지만, 경도와 위도 정보는 수동으로 입력해야 합니다. 초기 설정은 0으로 되어 있으며, 상단 상태 아이콘 위치에 빨간 GPS 아이콘이 표시됩니다. 예상 하늘을 제대로 그리려면 시간과 GPS 정보가 중요합니다.

Marker
------------------

eFinder 모드를 활성화하면 즉시 이미지에 빨간 표시가 나타납니다. 빨간 원의 중심은 메인 망원경이 보고 있는 지점입니다. 이 기능을 처음 사용할 경우, 이 마커를 이동시켜 망원경의 시야와 정렬시켜야 할 수 있습니다. 자세한 절차는 :ref:`eFinder Align <quickstart>` 를 참조하십시오.

Time Adjust
------------------

기본적으로 플래닛라리움은 현재 하늘을 보여줍니다. 하지만 타임 바를 조정하여 과거 및 미래의 하늘을 그릴 수 있습니다. 지원 범위는 현재 시간 기준 -10시간에서 +10시간입니다.

Star Finder |search|
--------------------------------

.. |search| image:: /images/search.png
                :scale: 40 %

Astroid에는 NGC, IC, M, HIP 별 목록이 내장되어 있습니다. Star Finder를 사용하려면 관심 있는 별 객체의 번호를 찾아 검색 창에 입력하십시오. 그러면 해당 별의 사진 및 기타 정보가 표시됩니다.

Star Finder 목록에서 별을 클릭하면 Astroid가 대상의 위치와 좌/우, 상/하 방향으로 얼마나 회전해야 하는지(도 단위)를 보여줍니다. 이 각도에 따라 마운트를 조정하세요. 현재 EQ 마운트 가이드라인은 지원되지 않지만, 이 기능은 향후 업데이트에서 추가될 예정입니다.

AR Mode |AR|
----------------------------------------

.. |AR| image:: /images/AR.png
                :scale: 10 %
                
기본적으로 화면을 드래그하면 항상 AzAlt 방향으로 이동합니다. 하지만 때때로 화면 뷰를 고정하고 세계를 움직이는 것이 편리할 때가 있습니다. 이 기능을 사용하려면 설정 메뉴에서 CameraView 옵션을 활성화하십시오.

Click and Find
-----------------------------------------------------

Astroid의 가장 독특한 기능 중 하나는 카메라 이미지에서 별과 DSO 정보를 클릭하여 찾을 수 있다는 점입니다. EAA 스태커와 결합하면, 목록에서 별을 선택하는 것보다 더 시각적으로 상호작용하는 방식으로 밤하늘을 탐험할 수 있습니다.

Camera Lock and Unlock |lock| 
----------------------------------------------------

.. |lock| image:: /images/lock.png
                :scale: 40 %

사용자 인터페이스는 기본적으로 카메라 이미지의 중심을 자동으로 따릅니다. 자동 카메라 추적 모드를 해제하려면 왼쪽의 잠금 버튼 |lock| 을 클릭하십시오.

버튼을 한 번 더 클릭하면 잠금 모드로 전환되어 다시 카메라를 따르게 됩니다.

Star List |starlist2|
----------------------------------------------------

.. |starlist2| image:: /images/starlist.png
                :scale: 40 %
                
Star Finder 창에서 추가 버튼 |add_to_list| 을 클릭하여 자신만의 별 목록을 만들 수 있습니다.

.. figure:: /images/searched_star.png
   :width: 200
   :alt: Max exposure
   :align: center

.. figure:: /images/auto_search.png
   :width: 400
   :alt: Max exposure
   :align: center

.. |add_to_list| image:: /images/add-list.png
                :scale: 40 %
                
추가된 별들은 Star List 창에서 볼 수 있습니다. Star List 창을 열려면 |starlist| 를 클릭하십시오.

.. |starlist| image:: /images/starlist.png
                :scale: 40 %

또한, |search_list| 아이콘을 클릭하여 현재 망원경 주변의 DSO를 자동으로 검색해 목록에 추가할 수 있습니다. 

|search_list| 근처의 DSO 검색. 기본적으로 M이 사용되지만, Astro Tools Menu에서 NGC, IC 등으로 변경할 수 있습니다.

.. |search_list| image:: /images/search_list.png
                :scale: 40 %

목록을 저장하고 불러오려면 다음 아이콘들을 사용하십시오.

|save_list| 목록 저장. 목록은 Astroid의 내부 메모리에 저장됩니다.

.. |save_list| image:: /images/save_list.png
                :scale: 40 %
                
|download_list| 목록 불러오기. 

.. |download_list| image:: /images/download_list.png
                :scale: 40 %

