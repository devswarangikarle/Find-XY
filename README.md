# Find-XY
You're given two integers, L and R.  Find if there exists two integers X and Y such that (L ≤ X &lt; Y ≤ R) and L ≤ LCM(X, Y) ≤ R or not. Print "YES" if these exists, "NO" Otherwise.  Note: LCM(x, y) be the minimum positive integer that is divisible by both x and y.

def find_XY(L, R):
    X = L
    Y = 2 * L
    
    if Y <= R:
        return "YES"
    else:
        return "NO"

L, R = map(int, input().split())

print(find_XY(L, R))
