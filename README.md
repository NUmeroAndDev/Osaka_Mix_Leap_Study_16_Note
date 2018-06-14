# [Osaka Mix Leap Study #16 - Android Jetpack 勉強会](https://yahoo-osaka.connpass.com/event/89865/)

## AndroidJetpack概要＆旧AACの紹介  
* LiveData  
setValue -> UiThread  
postValue -> Thread  
* LifecycleOwner  

```
val i = MutableLiveData

i.postValue
```

* ListAdapter DiffUtil  
submitList  
* ViewModel  (lateinit)  
View, Context参照しない
* Room  
基本は Thread から呼び出し  

## Navigation Architecture Component  



## [Deep Dive into Slice](https://speakerdeck.com/kobitokaba/deep-dive-into-slices?slide=1)  

