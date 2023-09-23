# [A2.Cheeseburger Corollary 2](https://www.facebook.com/codingcompetitions/hacker-cup/2023/practice-round/problems/A2)

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
    ll a, b, c, ans = 0;
    cin >> a >> b >> c;
    ll doubles = 0, singles = 0;
    if(b <= a * 2) {
        doubles =  c / b;
        ll rem = c - (doubles * b);
        if (rem >= a)
            singles++;
    }
    else {
        singles = c / a;
    }

    ll bread = doubles * 2 + singles * 2;
    ll meat = doubles * 2 + singles;
    ans = (bread == meat ? bread - 1 : meat);
    ans = max(ans, 0LL);
    cout << "Case #" << tc << ": " << ans << "\n";
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
