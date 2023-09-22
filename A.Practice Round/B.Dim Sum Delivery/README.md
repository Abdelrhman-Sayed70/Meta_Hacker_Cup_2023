# [B.Dim Sum Delivery](https://www.facebook.com/codingcompetitions/hacker-cup/2023/practice-round/problems/B)

![image](https://github.com/Abdelrhman-Sayed70/Meta_Hacker_Cup_2023/assets/99830416/59f3fe79-7b7e-4113-be5e-316bdc247c70)

## Solution

```cpp
#include<bits/stdc++.h>
using namespace std;
#define ll  long long
#define all(v) v.begin(),v.end()
void Go() {
    ios_base::sync_with_stdio(false), cin.tie(nullptr), cout.tie(nullptr);
    #ifndef ONLINE_JUDGE
        freopen("input.txt", "r", stdin);
        freopen("output.txt", "w", stdout);
    #endif
}
//*************
void doIt(int tc) {
    ll r, c, a, b;
    cin >> r >> c >> a >> b;
    cout << "Case #" << tc << ": ";
    cout << (c < r ? "YES\n" : "NO\n");
}
//*************
int main(){
    Go();
    int t = 1;
    cin >> t;
    for(int tc = 1; tc <= t; tc++)
        doIt(tc);
}
```
