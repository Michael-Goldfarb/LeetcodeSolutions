class Solution:
    def removeOuterParentheses(self, s: str) -> str:
        countB = 0
        result = ""
        for i in range(len(s)):
            if s[i] == '(':
                countB += 1
                if countB > 1:
                    result += s[i]
            elif s[i] == ')':
                countB -= 1
                if countB > 0:
                    result += s[i]
        return result