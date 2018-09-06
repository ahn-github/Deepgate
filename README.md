# Deepgate


  Deep Learning과 같은 연산량이 많은 응용분야에,  FPGA를 이용하여 처리속도를 향상시킬 수 있는 하드웨어 가속기를 만들고자 한다.
  
  장점
  1. FPGA는  네트워크 알고리즘을 언제든지 수정하여 다운로드 할수 있다.
  2. FPGA는 CPU보다 대략 100배 이상 빠르다
  3. FPGA는 GPU보다도 빠르며, 새로운 알고리즘을 다운로드 할 수 있으므로 훨씬 유연하다.
  4. USB3 / USB-C 인터페이스 형태로 만들면 기존의 대부분의 PC에서 사용할수 있다.
  5. USB단자를 가진 소형 CPU 모듈에도 적용가능하여, 수많은 독립현 지능 모듈에 적용가능하다.
  6. GPU보다 경제적이며 훈용기간이 훨씬 길어 환경 치화적이다.
  7. 전력 소비가 적다.
  
  
  
  
  구성도
  
                                          +----- MCU(D/L Control) 
                                          +        |
   USB3/USB-C -------  USB_Interface  ----+----- FPGA
                                                   +-------  HDMI_IO 
                                                   +-------  AUdio(I2S) -- Codec      
                                                   +-------  GPIO
                                                   +-------  Camera(Link)
                                                   +-------  USB(HUB)
                                                   +-------  Thunderbolt
                                                   +-------  SDcard_IF
                                                   
                                                   
  연산량이나 부하가 큰 명령을 FPGA에서 H/W적으로 처리                                                
   
  ex)     
       tf.add(x,y,name=None)
       tf.math.add
  
 https://www.tensorflow.org/api_guides/python/math_ops#Arithmetic_Operators
 
 
  
