YlSlide�õƲ��
---
### �����÷���

---

1��������jquery�⡢YlSlide�����������css�ļ�
```
<script type="text/javascript" src="js/jquery-1.9.1.min.js"></script>
<script type="text/javascript" src="js/jquery.Yl.Slide.min.js"></script>
<link rel="stylesheet" href="css/css.css" type="text/css">
```
2��JS����

```
			$(document).ready(function() {
				//�����÷�
				$('.Yl-container').YlSlide({
					wrapper:'.Yl-wrapper',//��װ��
					slideClass:'.Yl-slide',//ѭ����
					stylePrefix:'.Yl-',//ѭ���㸽����ʽǰ׺(��Ҫ�޸Ķ�Ӧ��CSSҲ���޸�)
					slideLength:3,//��ͼ����
					pages:true,//�Ƿ�����ҳ
					pagination:'.Yl-pagination',//��ҳ��ʽ
					pagingSelect:'.Yl-pagination-bullet-active',//��ҳѡ����ʽ
					autoplay:5000,//ÿ����ͼ�л�������	
					imgTemplate:{//ͼƬģ��
						0:['<div class="Yl-img0"></div>'],
						1:['<div class="Yl-img1"></div>'],
						2:['<div class="Yl-img2"></div>']
					},
					fontTemplate:{//����ģ��
					0:['<div class="Yl-font0">ALL ABOUT US</div>','<div class="Yl-font1">���ɾ��й��˵���ҵ��������ب�Ų����ʹ��</div>','<div class="Yl-font2">ֻΪһ�����</div>'],
					1:['<div class="Yl-font0">SINCE 2002</div>','<div class="Yl-font1">ʮ����רעһ����ѧ����ҵ��ٮٮ��</div>','<div class="Yl-font2">ֻΪһ�����</div>'],
					2:['<div class="Yl-font0">CHANCE FOR YOU</div>','<div class="Yl-font1">����Ч��ѧϰ��ʽ����ѧԱ���Ѹ��ٵ�ʱ��</div>','<div class="Yl-font2">ֻΪһ�����</div>']
					},
					fontAnimationMode:{//���ֶ���ģʽ
						0:['fadeInUp','fadeInUp','slideInLeft'],
						1:['fadeInUp','fadeInUp','slideInLeft'],
						2:['fadeInUp','fadeInUp','slideInLeft']
					},
					customTemplate:{//�Զ���ģ�壨��������ťģ�壩
						0:['<div class="Yl-Button"><a href="javascript:void(0);">����ר����ı���֮��</a></div>'],
						1:['<div class="Yl-Button"><a href="javascript:void(0);">����ר����ı���֮��</a></div>'],
						2:['<div class="Yl-Button"><a href="javascript:void(0);">����ר����ı���֮��</a></div>']
					},
					callback:function(e){//����DOM������ɺ�Ļص�����
												
					},
					before: function(e) {//ÿ����ͼ�л�ǰ�Ļص�����
						
					}, 
					after: function(e) {//ÿ����ͼ�л���ɺ�Ļص�����
						
					}
				});
			});


```
3.���沿��

```
<div class="Yl-container"></div>
```

---
### Ч��չʾ

1. ����չʾ[��https://yanliangnh.github.io/YlSlide/index.html](https://yanliangnh.github.io/YlSlide/index.html) 
2. һҳ����[��https://yanliangnh.github.io/YlSlide/multiScreen.html](https://yanliangnh.github.io/YlSlide/multiScreen.html)
3. cmd&amdģʽ[��https://yanliangnh.github.io/YlSlide/YlSlideSeajs.html](https://yanliangnh.github.io/YlSlide/YlSlideSeajs.html)

---

### �ص�����
```
callback:function(e){//����DOM������ɺ�Ļص�����
	//eΪ������������з��������ԣ���������console.log��e���鿴�����Լ���Ҫ�ģ�										
}
				
```


```
before: function(e) {//ÿ����ͼ�л�ǰ�Ļص�����
    //�˴���eΪ���Ƶ�ǰ��ͼ��
    //��ǰ��ţ�e.index
    //����ͼ��e.total
    //������װ���DOM����:e.ele
    //ֹͣ���ţ�e.pause()
    //��ʼ���ţ�e.play()
}
```

```
after: function(e) {//ҳ���л���ɺ�Ļص�����
    //ͬbefore�ص������÷�						
}
```



