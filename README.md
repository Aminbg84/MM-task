#include <iostream>
using namespace std;
int main () {
    int n, k, l, m, p;
    cout << "N = ";
    cin >> n;
    k=n; l=n, m=n, p=n;
    for (int i=0;i<(n+1)/2;i++) {
        for (int t=1;t<=2;t++) {
            for (int j=1;j<=k;j++) cout << '-';
            for (int j=1;j<=l;j++) cout << '*';
            for (int j=1;j<=m;j++) cout << '-';
            for (int j=1;j<=l;j++) cout << '*';
            for (int j=1;j<=k;j++) cout << '-';
        }
        cout << endl;
        k--;
        l+=2;
        m-=2;
    }
    l=1;
    m=n*2-1;
    for (int i=0;i<(n+1)/2;i++) {
        for (int t=1;t<=2;t++) {
            for (int j=1;j<=k;j++) cout << '-';
            for (int j=1;j<=n;j++) cout << '*';
            for (int j=1;j<=l;j++) cout << '-';
            for (int j=1;j<=m;j++) cout << '*';
            for (int j=1;j<=l;j++) cout << '-';
            for (int j=1;j<=n;j++) cout << '*';
            for (int j=1;j<=k;j++) cout << '-';
        }
        cout << endl;
        k--;
        l+=2;
        m-=2;
    }
    return 0;
}
