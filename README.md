# -nstaRoot-Bot
İnstaRoot-Bot instagramda takip botudur ve hesabınızda takipçi düşmesi olmadan takipçi kazanmanıza yarar

İşlevsellik: 

- **Info**: Raporu göster

- **Kullanıcıları takip et**: Etiketten, konumdan, bir listeden veya takip etmediğiniz kişileri geri takip edin

- **Kullanıcıları takip etmeyi bırak**: seni takip etmeyen ya da hepsi

---------------------

## Kullanım: 

**Raporu göster (takip eden, takibi bırakan, sizi geri takip eden):**
```
python main.py -u USERNAME -p PASSWORD -o info
```

**Tanıttığınız etiketi kullanarak kullanıcıları takip edin:**

```
python main.py -u USERNAME -p PASSWORD -o follow-tag -t TAG
```

**Kullanıcıları bir konumdan takip edin:**

```
python main.py -u USERNAME -p PASSWORD -o follow-location -t LOCATION_ID
```

**Geri takip etmediğiniz tüm kullanıcıları geri takip edin:**
```
python main.py -u USERNAME -p PASSWORD -o super-followback
```

**Bir listeden kullanıcıları takip edin:**

```
python main.py -u USERNAME -p PASSWORD -o follow-list -t USER_LIST
```

**Sizi takip etmeyen tüm kullanıcıları takibi bırakın:**
```
python main.py -u USERNAME -p PASSWORD -o super-unfollow
```
**Not**: "whitelist.txt" dosyasını asla takibi bırakmak istemeyeceğiniz hesaplarla doldurun


**Tüm kullanıcıları takibi bırak:**
```
python main.py -u USERNAME -p PASSWORD -o unfollow-all
```
**Not**: "whitelist.txt" dosyasını asla takibi bırakmak istemeyeceğiniz hesaplarla doldurun

---------------------

## Örnekler:

*python main.py -u USERNAME -p PASSWORD -o follow-tag -t cat* : **'Kedi' etiketini kullanarak kullanıcıları takip edin'** 

*python main.py -u USERNAME -p PASSWORD -o follow-location -t 127963847* : **İspanya'dan kullanıcıları takip edin** 

*python main.py -u USERNAME -p PASSWORD -o super-followback*: **Artık takip etmediğin ama seni takip eden kullanıcıları takip ediyorsun**

*python main.py -u USERNAME -p PASSWORD -o follow-list -t userlist.txt* : **userlist.txt dosyasının her satırındaki kullanıcıları takip edin** 

*python main.py -u USERNAME -p PASSWORD -o super-unfollow*: **Artık sizi takip etmeyen kullanıcıları takip etmiyorsunuz**
