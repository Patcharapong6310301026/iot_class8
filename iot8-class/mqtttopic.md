## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"flow level": "4"}
        - {"Rotating": "15"}
        - {"Dirt": "12"}
        - {"Vibration": "limit:30"}
        - {"Speed": "20"}
        - {"load": "2.3"}
        - {"cloth_weight": "1.6"}
        - {"detergent": "9"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"door detect": "on/off"}
        - {"radar": "2"}
        - {"remote sensor": "on"}
        - {"humidity": "31°C"}
        - {"current": "110"}
        - {"air_pressure": "1"}
        - {"cutout": "OFF"}



