# webpack 4.X �����������ò���



## һ����������

1����������Ŀ¼��E:\webpack\webpack_test���� 
2����ʼ������Ŀ¼��npm init�� 
3��ȫ�ְ�װwebpack-cli�� 

?	`npm uninstall webpack-cli`
?	`npm install -g webpack-cli`

4��ȫ�ְ�װwebpack�� 

?	`npm uninstall webpack`
?	`npm install -g webpack`

5��webpack �Cmode development/production���д��������package.json������dev��build�Ľű�����ֻ������npm run dev/build��������ͬ�� 
6����webpack �Cmode development/production�ɴ�����������������

7��������������

webpack --mode development --watch --progress --display-modules --colors --display-reasons



## ����ʵ��˵��

1������src�ļ��У�������index.js����ļ���E:\webpack\webpack_test\src\index.js��

2���������������������ļ��������ɴ������ļ�main.js��E:\webpack\webpack_test\dist\main.js��

webpack �Cmode development/production

3������distͬ��Ŀ¼web�������д����ļ�index.html�ļ���E:\webpack\webpack_test\web\index.html��������Ӧ��main,js�ļ������������������У��鿴ҳ��Ч����

�����Ϻ�ֻҪdist��web�����ļ������ݼ���ʵ��ҳ��ļ�ʱ���ʡ�



## ����ע��

1��`webpack4.x`��`'./src/index.js'`��Ϊ���

2��`webpack4.x`�Ժ󣬴��ʱ��ָ���������ļ�����·�������Զ�Ĭ������dist������main.js�ļ��� 

Ҳ����ͨ��������ʽָ�����·������ñ��ã���

�����npx webpack hello.js --output-filename hello.bundle.js --output-path . --mode development 
eg��
webpack hello.js --output-filename hello.bundle.js --output-path E:\webpack\webpack_test  --mode development



## �ģ�������ݣ����Ҳ����ڣ�

1����װnode
node -v

npm -v

2����װ��ʹ��webpack
1���½��ļ���webpack/webpack_test
?	�ڸ��ļ��������� npm init
2���������ļ����°�װwebpack
npm install webpack --save-dev

