# 4.6
#define _CRT_SECURE_NO_WARNINGS 1
#include<iostream>

using namespace std;
//int main()
//{
//	double num1 = 5, num2 = 2;
//	double num3 = (double)num1 / num2;//强制转换
//	cout << num3 << endl;
//	return 0;
//}

//int main()
//{
//	int num = 1024;
//	//演示复合运算符
//	num += 90;// <==> num = num + 90;
//	num *= 90;// <==> num = num * 90;
//	num /= 90;// <==> num = num / 90;
//	num -= 90;// <==> num = num - 90;
//	num %= 90;// <==> num = num % 90;
//	cout << num << endl;
//	return 0;
//}

//int main()
//{
//	//C语言中，0表示假，非0表示真
//	//C++中，引入了布尔类型 bool  (java - boolean)
//	bool flag = true;//false
//	cout << boolalpha;
//	cout << "15>88吗？" << (15 > 88) << endl;
//	cout << "16<99吗？" << (16 < 99) << endl;
//	return 0;
//}
//
//int main()
//{
//	//cout << (4 & 5) << endl;
//	//cout << ~2 << endl;
//	//cout << (2 << 3) << endl;
//	cout << (64 >> 2) << endl;
//	return 0;
//}
#include<iomanip>
//int main()
//{
//	cout << setw(23) << "sizeof(char)=" << sizeof(char) << '\n';
//	cout << setw(23) << "sizeof(short)=" << sizeof(short) << '\n';
//	cout << setw(23) << "sizeof(int)=" << sizeof(int) << '\n';
//	cout << setw(23) << "sizeof(long)=" << sizeof(long) << '\n';
//	cout << setw(23) << "sizeof(long long)=" << sizeof(long long) << '\n';
//	cout << setw(23) << "sizeof(float)=" << sizeof(float) << '\n';
//	cout << setw(23) << "sizeof(double)=" << sizeof(double) << '\n';
//	cout << setw(23) << "sizeof(long double)=" << sizeof(long double) << '\n';
//	return 0;
//}

//int main()
//{
//	cout << !((18 + 45 % 3 * 5) > 16) << endl;
//	return 0;
//}
//
//int main()
//{
//	//三元运算符
//	int num = 5 > 6 ? 10 : 12;
//	//      ?   :
//	//5是否大于6，如果5大于6，就返回输出10，如果5小于6，就返回输出12
//	cout << "num=" << num << endl;
//	return 0;
//}

//int main()
//{
//	//使用程序判断用户输入的字符是否是合法的硬盘盘符
//	char pan = '\0';   //默认值设置为空字符
//	cout << "请输入一个字符，我来判断是否合法：";
//	cin >> pan;
//	//'A'~'Z'
//	//if (pan>=65&&pan<=65+25)
//
//	if (pan >= 'A'&&pan <= 'Z')
//	{
//		cout << "是合法盘符！" << endl;
//
//	}
//	else
//	{
//		cout << "不是合法盘符！" << endl;
//	}
//	return 0;
//}

//int main()
//{
//	//败家mm的购物车
//	double price_louis = 35000.0;
//	double price_hemes = 11044.5;
//	double price_chanel = 1535.0;
//	double total = 0;//总价
//	double zhekou = 0;//折扣
//	total = price_chanel + price_hemes + price_louis;
//	//如果总价大于5w就打七折，否则打九折
//	if (total > 50000)
//	{
//		//total *=0.7;
//		zhekou = 0.7;
//	}
//	else
//	{
//		//total *=0.9;
//		zhekou = 0.9;
//	}
//	total *= zhekou;
//	cout << "最终付款：" << total << endl;
//	return 0;
//}
//
//int main()
//{
//	//败家mm的购物车
//	double price_louis = 35000.0;
//	double price_hemes = 11044.5;
//	double price_chanel = 1535.0;
//	double total = 0;//总价
//	double zhekou = 0;//折扣
//	total = price_chanel + price_hemes + price_louis;
//	//如果购买的三种商品有一种商品单价大于1000
//	//或三种商品总金额大于5000，折扣率为30%
//	//否则没有折扣
//	if (price_chanel > 1000 || price_hemes > 1000 || price_louis > 1000 || total > 5000)
//	{
//		//折扣0.3
//		zhekou = 0.3;
//	}
//
//	total *= zhekou;
//	cout << "最终付款：" << total << endl;
//	return 0;
//}

int main()
{
	cout << "欢迎来到自主投胎系统！" << endl;
	cout << "请开始选择：" << endl;
	cout << " 1.我要投胎\n 2.退出" << endl;
	int a=0 ;
	cout << "您的选择是："<<endl;
	cin >> a;
	//1.我要投胎
	if (a == 1)
	{
		int m=0;
		cout << "您的自主投胎即将开始，请先选择性别：" << endl;
		cout << " 1.男娃 - 免费\n 2.女娃 - 50币" << endl;
		cout << "您的选择是：" << endl;
		cin >> m;
		//选择男娃
			if (m == 1)
			{
			cout << "恭喜您即将成为一名男娃！" << endl;
			//生存难度
			cout << "请选择您的生存难度：" << endl;
			int o;
			cout << " 1.简单（1w币）\n 2.中等（5000币）\n 3.困难（1000币）\n 4.深渊（免费）" << endl;
			cout << "您的选择是：" << endl;
			cin >> o;
			//选择深渊
			if (o == 4)
			{
				int p;
				cout << "恭喜您进入了深渊模式！" << endl;
				cout << "请选择您的出身：" << endl;
				cout << " 1.我爸是李Gang套装（10w币）\n 2.富二代（5w币）\n 3.官二代（5w币）\n 4.军二代（5w币）\n 5.穷逼（免费）" << endl;
				cout << "您的选择是：" << endl;
				cin >> p;
				//选择穷逼
				if (p == 5)
				{
					//选择技能
					cout << "请您选择技能：" << endl;
					int q;
					cout << " 1.赚钱（1w币）\n 2.把妹（1w币）\n 3.文艺（1w币）\n 4.技工（1w币）\n 5.泡面（500币）\n 6.毛都不会（免费）" << endl;
					cout << "您的选择是：" << endl;
					cin >> q;
					//选择毛都不会
					if (q == 6)
					{
						//选择长相
						cout << "请您选择长相：" << endl;
						cout << " 1.帅哥套装1（1w币）\n 2.帅锅套装2（1w币）\n 3.随机（免费）" << endl;
						int r;
						cout << "您的选择是：" << endl;
						cin >> r;
						//选择随机长相
						if (r == 3)
						{
							cout << "您随机到的长相实在是太丑了，惨绝人寰！" << endl;
							cout << "请问您是否要进行投诉环节？" << endl;
							int s;
							cout << " 1.投诉\n 2.不投诉" << endl;
							cin >> s;
							//投诉
							if (s == 1)
							{
								cout << "恭喜您投诉成功，获得一套更丑的疤痕套装！" << endl;
								cout << "投胎成功！！！" << endl;

							}
							//不投诉
							else
							{
								cout << "您脾气真好，那您就开启你丑陋的人生吧!" << endl;
								cout << "投胎成功！！！" << endl;
							}
						}
						//选择其他长相
						else
						{
							cout << "您的余额为零！" << endl;
							int n;
							cout << "您是否要充值？" << endl;
							cout << " 1.老子要充值\n 2.没钱不充" << endl;
							cout << "您的选择是：" << endl;
							cin >> n;
							//老子要充值！
							if (n == 1)
							{
								cout << "老子要充值" << endl;
								cout << "您钱包余额不足，建议您下次投胎！" << endl;
							}
							//没钱不充！
							else
							{
								cout << "没钱不充" << endl;
								cout << "没钱投什么胎！" << endl;
							}
						}
					}
					//选择其他技能
					else
					{
						cout << "您的余额为零！" << endl;
						int n;
						cout << "您是否要充值？" << endl;
						cout << " 1.老子要充值\n 2.没钱不充" << endl;
						cout << "您的选择是：" << endl;
						cin >> n;
						//老子要充值！
						if (n == 1)
						{
							cout << "老子要充值" << endl;
							cout << "您钱包余额不足，建议您下次投胎！" << endl;
						}
						//没钱不充！
						else
						{
							cout << "没钱不充" << endl;
							cout << "没钱投什么胎！" << endl;
						}
					}
				}
				//选择其他出身
				else
				{

					cout << "您的余额为零！" << endl;
					int n;
					cout << "您是否要充值？" << endl;
					cout << " 1.老子要充值\n 2.没钱不充" << endl;
					cout << "您的选择是：" << endl;
					cin >> n;
					//老子要充值！
					if (n == 1)
					{
						cout << "老子要充值" << endl;
						cout << "您钱包余额不足，建议您下次投胎！" << endl;
					}
					//没钱不充！
					else
					{
						cout << "没钱不充" << endl;
						cout << "没钱投什么胎！" << endl;
					}
				}

			}
			//选择其他生存难度
			else
			{
				cout << "您的余额为零！" << endl;
				int n;
				cout << "您是否要充值？" << endl;
				cout << " 1.老子要充值\n 2.没钱不充" << endl;
				cout << "您的选择是：" << endl;
				cin >> n;
				//老子要充值！
				if (n == 1)
				{
					cout << "老子要充值" << endl;
					cout << "您钱包余额不足，建议您下次投胎！" << endl;
				}
				//没钱不充！
				else
				{
					cout << "没钱不充" << endl;
					cout << "没钱投什么胎！" << endl;
				}
			}

			}
		//选择女娃
			else if (m==2)
			{
				cout << "您的余额为零！" << endl;
				int n;
				cout << "您是否要充值？" << endl;
				cout << " 1.老子要充值\n 2.没钱不充" << endl;
				cout << "您的选择是：" << endl;
				cin >> n;
				//老子要充值！
				if (n == 1)
				{
					cout << "老子要充值" << endl;
					cout << "您钱包余额不足，建议您下次投胎！" << endl;
				}
				//没钱不充！
				else
				{
					cout << "没钱不充" << endl;
					cout << "没钱投什么胎！" << endl;

				}
			}
		//不男不女
			else
			{
				cout << "暂不提供不男不女服务！" << endl;
				cout << "这边建议您还是别做人了！" << endl;
			}
	}

	
	//2.退出
	else if(a == 2)
	{
		cout << "完了！您无法当个人了！" << endl;
		cout << "欢迎下次投胎！" << endl;
	}
	return 0;
}

//int main()
//{
//	int choice = 1;//choice=7SS
//	switch (choice)
//	{
//	case 1:
//		cout << "您选择了战士！" << endl;
//	case 1:
//		cout << "您选择了猎人！" << endl;
//	case 2:
//		cout << "您选择了术士！" << endl;
//	case 3:
//		cout << "您选择了牧师！" << endl;
//	case 4:
//		cout << "您选择了圣骑士！" << endl;
//	default:
//		cout << "您选择了退隐山林！" << endl;
//
//	}
//	return 0;
//}

//int main()
//{
//	//判断某月有几天
//	int month = 12;
//	switch (month)
//	{
//	case 1:
//	case 3:
//	case 5:
//	case 7:
//	case 8:
//	case 10:
//	case 12:
//		cout << "31天" << endl;
//		break;
//	case 2:
//		break;
//		//……
//	}
//}
//
//int main()
//{
//	//强调下if的大括号
//	int a = 5, b = 10;
//	if (a > b)
//	{
//		if (a++ > --b)
//		{
//			a += b;
//		}
//	}
//	cout << a << '\t' << b << endl;
//}
//
//int main()
//{
//	//强调下if的大括号
//	int num = 5;
//	cout << sizeof(num++) << endl;//4
//	cout << num << endl;//5
//}
