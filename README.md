#### ʵ�ֹ��ܣ�

###### ����һ��WebPack��loader��ʵ��html����pug�ļ�תΪjsģ�飬���ڿ���ģ������ǰ�����������ʵ���﷨������


##### ʹ�ò���ͼʾ
![](1.png)

##### ʹ�ò�����ϸ
###### 1. ��װloaderģ��
npm install html-pug-to-js-loader --save-dev
###### 2. webpack loader����

      {
        test: /\.(pug|html)$/,
        loader: 'html-pug-to-js-loader',
        query: {
          wrap: 'es6'
        }
      },
      
###### 3. ������ʹ��

```
import tpl from './b.pug';
import t  from './c.html';
var e = require('./b.pug');
var h = require('./b.html');
```

##### 4. ����ʾ��ͼ
###### HTMLתΪJS
![](2.png)
###### PugתΪJS
![](3.png)

##### 5. ע������
###### query��wrap��������ѡֵ es6 �� commonjs 
![](4.png)