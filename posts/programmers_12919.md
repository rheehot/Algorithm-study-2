## 문제
- 프로그래머스 : 서울에서 김서방 찾기
- https://programmers.co.kr/learn/courses/30/lessons/12919

<br/>

## 풀이
- string, append 만 안다면 1분만에 풀 수 있는 문제 

<br/>

## 코드

```c++
#include <string>
#include <vector>

using namespace std;

string solution(vector<string> seoul) {
    string answer = "김서방은 ";
    
    for(int i=0; i<seoul.size(); i++){
        string ans = "Kim";
        if(ans.compare(seoul.at(i)) == 0){
            answer.append(to_string(i));
        }
    }
    
    answer.append("에 있다");
    return answer;
}
```

<br/>

## 반성

- string 관련 내장 함수를 잘 기억 하자 

```c++

    a.compare(b) == 0 // 문자열이 같은 경우
    
    string str = to_string(i); // int to string 
    
```


<br/>


## screenshot

![screenshot](./screenshots/prog_김서방.png)
