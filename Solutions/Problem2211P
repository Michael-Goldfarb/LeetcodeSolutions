class Solution:
    def countCollisions(self, directions: str) -> int:
        ans = 0
        # At the beginning, leftest car can go without collide
        # At the beginning, rightest car can go without collide
        
        leftc = rightc = 0
        
        for c in directions:
            # if left side, no car stop or right answer + 0
            # if left side start to have car go right or stop
            # then cars after that are bound to be stopped so answer + 1
            if c == "L":
                ans += leftc
            else:
                leftc = 1
                
        for c in directions[::-1]:
            # if right side, no car stop or left answer + 0
            # if right side start to have car go left or stop
            # then cars after that are bound to be stopped so answer + 1
            if c == "R":
                ans += rightc
            else:
                rightc = 1
       
        return ans