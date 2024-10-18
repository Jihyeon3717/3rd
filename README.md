![image](https://github.com/user-attachments/assets/f0f819a0-1df3-4d89-b9b3-2b71c8a411f7)# AIFFEL Data Scientist Campus Code Peer Review Templete

코더 : 김진형

리뷰어 : 손지현

---

🔑 **PRT(Peer Review Template)**

[✅]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
- 최종 결과물 첨부되었습니다. 입출금 내역을 출력하는 method에서 오류가 발생합니다.   
![image](https://github.com/user-attachments/assets/c1ebd08d-c136-4a10-b45a-e28a2b5be64b)
    
[✅]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
	주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**

- 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
- 가장 핵심적인 부분은 계좌번호를 생성하는 메서드, 입금 메서드, 출금 메서드이고, 복잡한 부분은 이자 지급 메서드라고 생각합니다. 해당 코드 블럭에는 간단하게 주석이 작성되어 있습니다.  
  ![image](https://github.com/user-attachments/assets/f2d17b94-d872-4879-bf8b-7148f8a9cdd9)

- 입금 메서드는 if-else 조건문을 이용하여 조건을 만족할때(입금금액이 1원이상일때) balance에 합산됩니다. 또한 입금 내역을 합산하는 변수에도 합산됩니다.  
- 또한, 입금횟수가 5회일때 이자가 지급되도록, if self.deposit_count % 5 == 0: 부분도 작성된 것을 확인하였습니다.   
        
[✅]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록"을 남겼거나 "새로운 시도 
또는 추가 실험"을 수행해봤나요?**
- 자세한 기록은 확인할 수 없지만 문제를 해결하기 위해 노력하신 부분이 보입니다.
        
[✅]  **4. 회고를 잘 작성했나요?**
- 입금, 출금 내역의 코드에서 오류가 나는 것을 확인할 수 있습니다.
- Account 객체에 deposit_history_list 속성이 정의되지 않았기 때문에 발생하는 것으로 보입니다.
- Account 클래스의 생성자 (__init__)에서 해당 속성을 초기화를 해주면 해결할 수 있을 것 같습니다.

[✅]  **5. 코드가 간결하고 효율적인가요?**
- 코드의 대부분의 내용이 클래스에 포함되어있고, 클래스가 아닌 부분도 함수로 잘 적혀있어 효율적입니다. 

---
### 참고 문헌
