# MyFramework v1.0.0
MyFramework �� Asp.NetCore С����Ŀ���ٿ�����ܡ�Ŀǰ�����ݲִ���������Ԫ��������ƣ� Services��dto���������������˼򵥵ķ�װ�������ܴﵽ�ܿ��ٿ������ֲ�ʧ����ԡ�

����̨����ϵͳ demo: https://github.com/niaiaiai/BookStoreDemo

����̨����ϵͳǰ�� demo: https://github.com/niaiaiai/BookStoreDemoWeb

demo: https://studydemo.online:8081/

## �������д�����Ŀģ��
    dotnet new -i MyFramework.Templates --nuget-source http://studydemo.online:13564/v3/index.json
    dotnet new Myfw -n [��Ŀ����]

## ��Ŀ�ṹ
ddd �ܹ�

* Application Ӧ�ò�
* Domain �����
* Infrastructure ������ʩ��
* Web web ��
* Ids4 IdentityServer4 ��֤��Ȩ���������ɵ�������

* ApplicationTest Ӧ�ò������Ŀ
* DomainTest ����������Ŀ
* InfrastructureTest ������ʩ�������Ŀ
* WebTest web �������Ŀ
* TestBase ������Ŀ�Ļ���

* docker-compose Web ��Ŀ�� docker �����ļ�
* Web/Dockerfile ���� docker ����
* nuget.config nuget �ֿ�����

## ���ݿ�Ǩ��
ʵ�� IDataSeed �ӿں󣬻��Զ�Ǩ�Ʋ���ʼ�����ݡ�

Package Manager ����:
```
PM> Add-Migration Init -Context XXXContext -Project Infrastructure -StartupProject Infrastructure -Args '--environment Development'
PM> Update-Database -Context XXXContext -Project Infrastructure -StartupProject Infrastructure -Args '--environment Development'
```

������������������Ŀ�������ļ�����:
```
-Args '--environment Development' �� -Args '--environment Production'
```

## ��������Ŀ
���� baget �ֿ��ַ: http://studydemo.online:13564/

* Utils                  �����࣬��������
* MyServices             Service �ķ�װ    ע�볣�õĽӿڣ���װ��ҳdto
* MyRepositories         �ִ���������Ԫ     ���Զ��ύ���񣬲ִ��ο�abp
* MyEntityFrameworkCore  DbContext ����    ��װ����ɾ����������ƵĹ���
* MyEntity               ʵ����࣬������� �����������������ݵ���ƣ���ɾ��
* MyAuthorization        IdentityServer4 �� web ��Ŀ ��ʱδʹ��

## ����������
* AutoMapper
* IdentityServer4

## ��Ŀά��
���ڿ�ܴ��ڳ�ʼ�׶Σ��Ժ����ά�������ƿ�ܡ�