//Taikinys
#include <iostream>
#include <iomanip>
#include <cmath>
using namespace std;
int main ()
{
 double xc, yc, // taikinio centro koordinatės
 r1, r2, r3, r4; // taikinio apskritimų spinduliai didėjimo tvarka
 int t1, t2, t3, t4; // skiriami taškai atsižvelgiant į apskritimus
 double x, y, ats, tiks; // strėlės pataikymo taško koordinatės
 // Duomenų skaitymas
 cout << "Taikinio centro koordinate xc = "; cin >> xc;
 cout << "Taikinio centro koordinate yc = "; cin >> yc;
 cout << "Pirmojo apskritimo spindulys r1 = "; cin >> r1;
 cout << "Pirmojo apskritimo taskai t1 = "; cin >> t1;
 cout << "Antrojo apskritimo spindulys r2 = "; cin >> r2;
 cout << "Antrojo apskritimo taskai t2 = "; cin >> t2;
 cout << "Treciojo apskritimo spindulys r3 = "; cin >> r3;
 cout << "Treciojo apskritimo taskai t3 = "; cin >> t3;
 cout << "Ketvirtojo apskritimo spindulys r4 = "; cin >> r4;
 cout << "Ketvirtojo apskritimo taskai t4 = "; cin >> t4;
 cout << "Streles koordinate x = "; cin >> x;
 cout << "Streles koordinate y = "; cin >> y;
 ats = sqrt((xc - x) * (xc - x) + (yc - y) * (yc - y));
 cout << "Ats - " << ats << endl;
 tiks = ats / xc / yc / 100;
 cout << "Tikslumas: " << setw(8) << fixed << setprecision(5) << tiks << endl;
return 0;
}
