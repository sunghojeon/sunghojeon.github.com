---
layout: post
title: ATSC3.0 방송장비 동향 / KOBA2016 출품장비를 중심으로 
---

**[알림] 본 원고는 한국방송기술인연합회 ['방송과 기술' 7월호](http://tech.kobeta.com/%EB%B0%A9%EC%86%A1%EA%B3%BC%EA%B8%B0%EC%88%A0-2016%EB%85%84-7%EC%9B%94%ED%98%B8vol-247-%EC%95%88%EB%82%B4/)에 출판되었습니다.**

## 송신장비 동향

2017년 2월 본방송을 위해서는 우선 각 송신소에 설치해야하는 고출력 송신기, 권역별로 단일 주파수 방송망(Single Frequency Network; SFN)을 제어하기 위한 Broadcast Gateway 장비, 그리고 장비들을 이중화하고 개별 장비들의 상태를 실시간으로 모니터링 할 수 있는 장비가 필요하다.

![그림 1](/images/KOBA2016_Equipment_1.JPG)

#### 엑사이터 Exciter [A321+A322]

물리계층 전송 표준의 경우, ATSC3.0 전체 표준들 가운데 가장 먼저 확정되었고, 표준안을 바탕으로 제조사들 상호 간 송수신 정합(PlugFest)도 2차례나 실시하여, 기술의 완성도가 높다고 할 수 있다. 하지만, KOBA2016에 전시된 엑사이터들은 LDM(Layer Division Multiplexing) 기술을 아직까지 지원하지 않고 있었다.

기존 MPEG2-TS 스트림을 ASI 포트로 입력을 받던 ATSC1.0 장비들과 달리, ATSC3.0 송신장비들은 ALP(ATSC Link Protocol) 스트림을 IP 포트로 입력을 받는다는 점이 큰 특징이다. 따라서, 엑사이터 장비 공통적으로 2개의 IP Port로부터 이중화된 입력을 받을 수 있게 제작되었고, 신호의 입력을 감지하여 자동절체(Seamless Switching)하는 기능을 지원하고 있었다. 

추후, 송신기 도입 시에는 신호 절체 기준 및 시점에 대해서는 각 방송사 별 내부 기준에 따라 조정이 필요할 것으로 예상되며, 실제 네트워크 구축 시에는 송신기 입력 IP 경로 차이에 따른 지연시간을 자동절체 시 보상해주어 송신기 전체 SFN Delay를 일정하게 유지시킬 수 있는지 확인이 필요하다.

![그림 2](/images/KOBA2016_Equipment_2.JPG)


#### Broadcast Gateway [A324]

SFN 송신기 제어를 위해서 필수적인 Broadcast Gateway 장비의 경우, 각 제조사들이 시제품Prototype을 만들어 전시하였다. 전시 장비들에서 공통적으로 확인할 수 있는 점은, 기능적으로 복잡해진 ATSC3.0 물리계층 송신 파라미터를 설정하기 위한 그래픽 기반 사용자 인터페이스(GUI; Graphical User Interface)를 제공한다는 점이다. 이러한 설정 역시 IP망으로 연결되어서 중앙집중식 제어 및 관리가 가능하다.

전시 장비들이 시제품인 이유는, 2016년 7월 초안 완성을 목표로 A/324 표준화 작업이 진행 중이기 때문에 아직까지 확정된 표준이 없어, 제조사별로 자체 방식으로 구현되었기 때문에, 같은 회사 제품끼리는 동작하지만, 타사 제품들과의 호환이 이루어지지 않는 점 때문이다. 따라서, 제조사들은 공통적으로 본방송을 위한 Broadcast Gateway 장비는 표준이 확정되고 난 후인 12월경으로 예측하고 있으며, 상용 제품이 출시된 후에는 다양한 종류의 Exciter와 Broadcast Gateway 조합을 대상으로 충분한 연동실험이 필요하다는 데 의견을 같이 하였다.

※ 참고로, DVB-T2 SFN을 구성한 KBS의 경우, ENENSYS T2-Gateway 장비를 여의도 본사에 설치하고, 관악산송신소와 남산송신소에 각각에 Rhode&Schwartz Exciter를 설치한 뒤 연결하여 실험방송 중에 있다.


#### 방송망 원격 제어/모니터링 시스템 

송신기들이 IP 기반으로 동작하기 때문에, 장비들 각각이 고유한 IP Address를 가지게 되고, 이 때문에 장비들을 인터넷에 연결시키기만 하면, 개별 장비들에 직접 접속하여 원격으로 상태를 파악하고 제어하는 것이 가능해졌다. 또한, 실시간으로 수집되는 장비들의 상태를 그래픽 기반 화면으로 일목요연하게 표출함으로써, 운용자들이 각종 정보를 쉽게 파악할 수 있게 함은 물론 운용의 편의성을 높이기 위해 노력하고 있었다.


![그림 3](/images/KOBA2016_Equipment_3.JPG)



