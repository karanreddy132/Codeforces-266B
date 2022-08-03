# Codeforces-266B
#include <bits/stdc++.h>
using namespace std;

int main() {
	int n,t;
  string s;
  cin >> n >> t;
  cin >> s;
	for (int j = 0; j < t; j++) {
		for (int i = 0; i < s.size() - 1; i++) {
			if (s[i] == 'B' && s[i + 1] == 'G') {
				s[i] = 'G';
        s[i+1] = 'B';
				i++;
			}
		}
	}
	cout << s;
	return 0;
}
