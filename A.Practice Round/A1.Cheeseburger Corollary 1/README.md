# [A1.Cheeseburger Corollary 1](https://www.facebook.com/codingcompetitions/hacker-cup/2023/practice-round/problems/A1)

![image](https://github.com/Abdelrhman-Sayed70/Meta_Hacker_Cup_2023/assets/99830416/4505025d-3b79-4a57-811f-ed61308ba13e)

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
    int s, d, k;
    cin >> s >> d >> k;

    int bread = (s * 2) + (d * 2);
    int chees = s + (2 * d);
    int meat = s + (2 * d);
    bool valid = (bread >= k + 1) && (chees >= k) && (meat >= k);

    cout << "Case #" << tc << ": ";
    cout << (valid ? "YES\n" : "NO\n");
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
