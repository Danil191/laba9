# laba9


Введеение размера матриц
C++



#include "windows.h"
#include <iostream>
using namespace std;
int main()
{
  SetConsoleCP(1251);
  SetConsoleOutputCP(1251);
    int n,m;
    int posF = 0,posG = 0;
    cout << "Введите размер произвольной матрицы F:" << endl;
    cin >> n;
    cin >> m;
    int F[n][m];

    for (int i=0;i<n;i++)
    {
        for (int j=0;j<m;j++)
        {
            cout << "Введите элемент матрицы F[" << i+1 << "][" << j+1 << "]:";
            cin >> F[i][j];
        }
    }

    for  (int i=0;i<n;i++)
        for(int j=0;j<m;j++)
        if (F[i][j]>0)
            posF = posF + 1 ;


    cout << "Введите размер произвольной матрицы G:" << endl;
    cin >> n;
    cin >> m;
    int G[n][m];

    for (int i=0;i<n;i++)
    {
        for (int j=0;j<m;j++)
        {
            cout << "Введите элемент матрицы G[" << i+1 << "][" << j+1 << "]:";
            cin >> G[i][j];
        }
    }
    int i=0;
    int j=0;
    for  (int i=0;i<n;i++)
        for(int j=0;j<m;j++)
        if (G[i][j] >0)
            posG = posG + 1 ;

    cout << "Количество положительных элементов в матрице F:" << posF << "\n";
    cout << "Количество положительных элементво в матрице G:" << posG;

    return 0;
}

