# <h1 align="center"> Exorde </h1>


![image](https://user-images.githubusercontent.com/101149671/201298361-b48bc53b-7858-42c2-b6ab-5cf7270e3429.png)

<h1 align="center"> Selamlar, Coinlist tarafından desteklenen ExordeLabs testnet rehberi, aşağıda gerekli linkler ve rehber mevcut:
</h1>

### Linkler:

 * [Exorde Türkiye Kanalı](https://t.me/ExordeTurkish)
 * [Exorde Discord Kanalı](https://discord.gg/44KzbSWB)
 * [Sıralama](https://explorer.exorde.network/leaderboard) ve [Explorer](https://explorer.exorde.network/)
 * Video rehberi gün içinde gelecek
 * Sohbet ve sorular için [Discord](discord.gg/ruescommunity) ve [Telegram](https://t.me/RuesChat) kanallarımız

## NOT (ilk defa node kuranlar):

 * Bu nodeları bilgisayarınıza kurabilirisniz ancak tavsiye etmem asla
 * Sanal sunucu kullanıyoruz, ücretli/ücretsiz sunucular mevcut.
 * Discord kanalımda sunucu nedir, node nedir, nasıl bağlanılır bu 3 temel konu hakkında video ve makale mevcut
 * Bunları anladığınız anda tüm nodeları kendiniz kurabilirsiniz, sorularınız için discord kanalı mevcut.
 * Rehberler ve sorular için: [Discord kanalı](discord.gg/ruescommunity)

## Sistem gereksinimi:

 * Net bilgi yok, kendim test ettim:

```
CPU : 2 cores
RAM: 4Gb
SSD: 20Gb
```
## Docker ve güncellemeler::

```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
```

## Screen:
```
sudo apt install -y build-essential libssl-dev libffi-dev git curl screen
```

## Git clone çekiyoruz
```
git clone https://github.com/exorde-labs/ExordeModuleCLI.git
```

## Burası uzun bir yükleme sürecek:
```
cd ExordeModuleCLI
docker build -t exorde-cli .
```

## Bir screen açıyoruz:
```
screen -S exorde
```

## Metamask yazdığım yere 0xli başlayan metamask adresi giriyoruz:

 * Testnet cüzdanı kullanın

```
docker run -it exorde-cli -m metamask -l 2
```



## Gerekli komutlar:

 * Screen açma:

```
screen -S screenadı
```

 * Screen içersine girme:

```
screen -r screenadı
```

 * Screenleri görme:

```
screen -ls
```

 * Screen silme:

```
screen -XS screenadı quit
```

 * Tüm screenleri silme:

```
pkill screen
```







