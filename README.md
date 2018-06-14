# [Osaka Mix Leap Study #16 - Android Jetpack 勉強会](https://yahoo-osaka.connpass.com/event/89865/)

## [AndroidJetpack概要＆旧AACの紹介](https://speakerdeck.com/katsukinakatani/androidjetpackgai-yao-jiu-aacfalseshao-jie?slide=1)  
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

## [Navigation Architecture Component](https://www.slideshare.net/yasi_life/navigation-architecture-component)  
* BottomNavigation と併用の場合 navigation-ui  
* Destination (Fragment or Activity のこと)  
* Activity -> NavHost  
* NavConstroller で遷移とか  
* navigation-ui  
navigation の xml の id を menu の id にする  
* safe-args-gradle 
遷移元fragment名 + Directionsが生成される  
      
## [Deep Dive into Slice](https://speakerdeck.com/kobitokaba/deep-dive-into-slices?slide=1)  
* テンプレート化された UI  
* Jetpack 側で諸々更新される  
* Slice 自体は構造化されている  
* ContentProviderClient   
毎回 ContentProvider をアクセスしないためのもの  
* 2 秒以内に Slice を返さないといけない
読み込み中を返して非同期で表示させる?


