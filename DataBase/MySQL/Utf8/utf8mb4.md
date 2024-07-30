MariaDB등 

utf8은 utf8mb3 세팅이다 ( 3byte )

따라서 일부 이모지와 같은 utf8mb4 (4byte) string을 저장하는데 문제가 있다. 

# 해결법
// 4byte를 넘는 문자를 탐색
export const RegexFind4Bytes  = /[\uD800-\uDBFF]|[\uDC00-\uDFFF]/;

// 일어 + 한자 + 영어 + 숫자 + 특수기호(키보드에 있는)만 제외하고 탐색
export const RegexForbidden = /[^0-9^a-z^A-Z^ぁ-ん^ァ-ン^一-龯^!@#$%^&*()_\+\-={}\[\]\\|;:'\",.<>\/?\s]/;