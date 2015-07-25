### IT12068838 ##
### W.V.H.Malinga ##

----------


# Creating an Amazon EBS-Backed Linux AMI #
------------------------------------------
## To create an AMI from a snapshot using the console ##

###1. Open the Amazon EC2 console. ###
![01](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/11742794_968171139895157_2342155509294809689_n.jpg?oh=16fb0cd91eeecf63c9620fcae490e50a&oe=56467685)

###2. Connect to the instance and customize it. ###
![02](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xtf1/v/t1.0-9/11745723_968171136561824_5705064340824620841_n.jpg?oh=7129a0ef3b91fb7efd6d225d3f86e608&oe=560F81DF)

![03](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpt1/v/t1.0-9/11755211_968171183228486_1900518593525869964_n.jpg?oh=c966b58ee774027a701e28dad9ccbca7&oe=564EDD1D)

![04](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xfp1/v/t1.0-9/11015479_968171216561816_899023273401057581_n.jpg?oh=dc1f4688df488a9f1e5261d1210961a2&oe=5657D4A7)

### 3. In the navigation pane, click Instances and select your instance. Click Actions, select Image, and then click Create Image. ###
![05](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpa1/v/t1.0-9/11228107_968171179895153_2862103353930795424_n.jpg?oh=721d5cabf6a9d99051e3d7ab75e1bc7a&oe=560EC0D2)

### 4. In the Create Image dialog box, specify the following, and then click Create Image. ###
1. A unique name for the image.
2. A description of the image, up to 255 characters.
3. By default, Amazon EC2 shuts down the instance, takes snapshots of any attached volumes, creates and registers the AMI, and then reboots the instance. Select No reboot if you don't want your instance to be shut down.
![06](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpt1/v/t1.0-9/11751769_968171226561815_456204463398377642_n.jpg?oh=5f7775d8808a9f5383cd0c3ed2e01381&oe=5642696F)

![07](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xta1/v/t1.0-9/11800258_968171236561814_5661177062011354479_n.jpg?oh=2f65ae5fa22a4be7ab95c39998785578&oe=56599344)

### 5. Click AMIs in the navigation pane to view the status of your AMI. While the new AMI is being created, its status is pending. This process typically takes a few minutes	to finish, and then the status of your AMI is available. ###
![08](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xap1/v/t1.0-9/11737885_968171276561810_8886580051366971915_n.jpg?oh=b586d6c730a76b35de94dfc6400041ea&oe=56464145)

![09](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpf1/v/t1.0-9/11032481_968171283228476_6576107575408240206_n.jpg?oh=a45adef720b36e35a9d2b70529b5438f&oe=5640E711)

## Creating a Linux AMI from a Snapshot ##

###1. In the navigation pane, under Elastic Block Store, choose Snapshots. ###
![10](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xpt1/v/t1.0-9/11796395_968171306561807_4778082085619138740_n.jpg?oh=0aed7c9d3deb304b55169ad5ca4a2a7f&oe=565A9762)

### 2. Choose the snapshot, and then choose Create Image from the Actions list. ###
![11](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xft1/v/t1.0-9/11753653_968171313228473_1442508442738127679_n.jpg?oh=d0923937a63977db90dfba1290ad39fa&oe=56507155)

![12](https://scontent-ams3-1.xx.fbcdn.net/hphotos-xft1/v/t1.0-9/11751769_968171349895136_3783218384397243932_n.jpg?oh=e648cf11523e6e67c58642b52160aa0e&oe=5658DCA9)