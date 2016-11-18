# C-
This is in the book
// 例5-10.cpp : 定义控制台应用程序的入口点。
//this指针查看私有数据

#include "stdafx.h"
#include<iostream>
using namespace std;

class Text
{
public:
	Text(int i) { a = i; }//构造函数
	void print()
	{
		cout << "a=" << a << endl;
		cout << "this->a=" << this->a << endl;
		cout << "this=" << this << endl;
	}
private:
	int a;
};

void main()
{
	Text x1(100);
	Text x2(200);
	x1.print();
	x2.print();
	system("pause");
}
