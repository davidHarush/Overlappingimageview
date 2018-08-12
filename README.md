# Overlappingimageview
Simple custom ImageView for android

Imageview with simple way to enable overlapping of two images one over the other.<br/>
This project helped me build a gallery with multiple selection modes.<br/>
You can use a Drawable or xml shape in front of or behind the regular ImageView resource.<br/>
The Drawable will resize according to the ImageView size.<br/><br/>

<img style="border: 1px solid black;float:left;" src="https://github.com/davidHarush/Overlappingimageview/blob/master/Screenshot.png" width="168" height="auto" hspace="30" />
<img style="border: 1px solid black;float:left;" src="https://github.com/davidHarush/Overlappingimageview/blob/master/Screenshot_1.png" width="168" height="auto"  hspace="30" />
<img style="border: 1px solid black;float:left;" src="https://github.com/davidHarush/Overlappingimageview/blob/master/Screenshot_2.png" width="168" height="auto"  hspace="30" />

<br style="clear: both;" />
<br/>
<b>How to use:</b> all you need to do is to copy <i>OverLappingImageView.java</i> to your project and start using it.
<br/>
<br/>
<b>Code examples:</b>
<br/>
<br/>
exmple for drawble mask draw in front of the image:

```
OverlappingImageView  mImg1 = ((OverlappingImageView) findViewById(R.id.imageView1));
mImg1.setMaskShape(R.drawable.mask_shape);
mImg1.setDrawOnFront(true);
```

<br/>
exmple for drawble mask draw behind of the image:

```
OverlappingImageView mImg2 = ((OverlappingImageView) findViewById(R.id.imageView2))
                .setMaskShape(android.R.drawable.picture_frame)
                .setDrawOnFront(false);
```

after init you can use:

```
mImg2.toggleMask();
```

or 

```
mImg2.showMask(true);
```

<br/><br/>
Download the sample app form Google Play:
<br/>
<a href='https://play.google.com/store/apps/details?id=com.david.Overlappingimageview&utm_source=global_co&utm_medium=prtnr&utm_content=Mar2515&utm_campaign=PartBadge&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'  width="168" height="60" /></a>

