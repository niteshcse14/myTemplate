```cpp
/*
	Name 		: 	Nitesh Meena
	Company		:	Backend Developer at Codalien
	Email		: 	nitesh.cse14@nituk.ac.in
	College		:	National Institute of Technology, Uttarakhand
*/
#include <iostream>
#include <vector>
#include <cstring>
#include <cstdarg>
#include <string>
using namespace std;

typedef long long int 				ll;
typedef unsigned long long int 		ull;
typedef vector<int> 				vi;
typedef vector<ll> 					vl;
typedef vector<vi> 					vii;
typedef vector<vl> 					vll;

typedef pair<int, int> 				pii;
typedef pair<ll, ll> 				pll;

#define maxn 						1000010
#define MOD 						1000000007
#define INF 						2173641287
#define For(i, a, b) 				for (int i = a; i <= b; ++i)
#define Ford(i, a, b) 				for (int i = a; i <= b; --i)
#define f 							first
#define s 							second
#define pb 							push_back

#define sf(a) 						cin >> a;
#define sff(a, b) 					cin >> a >> b;
#define sfff(a, b, c) 				cin >> a >> b >> c;


void pf() {
	printf("\n");
}
template <class T, class... Types>
void pf(T val, Types... args) {
	cout << val << " ";
	pf(args...);
}

template <class T, class U>
class Nitesh {
private:
	T t, n, m, mx, temp, res;
	U *inp, *pat, *text;
	T *lps;
public:
	Nitesh() {
		pf("Loading...... class Nitesh");
		pf("Enter Number of test cases");
		sf(t);
	};
	void solve();

	void doFast() {
		ios_base::sync_with_stdio(false); 
	    cin.tie(NULL); 
	}

	void takeArrayInput(T n, U arr[]) {
		for (T i = 0; i < n; ++i)
			sf(arr[i]);
	}

	void takeArrayInput(T n, T arr[]) {
		for (T i = 0; i < n; ++i)
			sf(arr[i]);
	}

	void printArray(T n, T arr[]) {
		for (T i = 0; i < n; ++i)
			cout << arr[i] << " ";
		pf();
	}
	void printArray(T n, U arr[]) {
		for (T i = 0; i < n; ++i)
			cout << arr[i] << " ";
		pf();
	}
	T max(T x, T y) {
		return (x > y) ? x: y;
	}
	T min(T x, T y) {
		return (x < y) ? x: y;
	}
	T pow(T x, T y) {
		T res = 1;
		while (y) {
			if (y & 1) res = res * x;
			x = x * x;
			y /= 2;
		}
		return res;
	}

	T modPow(T x, T y) {
		T res = 1;
		while (y) {
			if (y & 1) res = (res * x + MOD) % MOD;
			x = (x * x + MOD) % MOD;
			y = y / 2;;
		}
		return res % MOD;
	}
	T gcd(T x, T y) {
		if (y == 0) return x;
		return gcd(y, x % y);
	}
};

// do something for external functions

template<class T, class U>
void Nitesh<T, U>::solve() {
	pf("Loading...... Solve Class");
	for (T test = 0; test < t; ++test) {
		pf("Running for test case ", test);
		//
	}
}

int main(int argc, char const *argv[]) {
	Nitesh<int, char> nitesh;
	//nitesh.doFast();
	nitesh.solve();
	return 0;
}
```