##### Formato (.aab)
Android App Bundle é um formato de publicação que inclui todos os recursos e códigos compilados do seu app. O Google PLay usa o pacote de app para gerar e disponibilizar APKs otimizados para cada configuração de dispositivo. Isso permite que os usuários baixem um APK menor.

#### Formato (.apk)
Ele é um pacote complete que contém todos os recursos e códigos do aplicativo em um único arquivo. O APK é compilado para cada arquitetura alvo, como ARM, ARM64, x86, etc. Como resultado, o tamanho do APK pode ser maior em comparação com um arquivo .aab, pois contém todos os recursos para todas as arquiteturas suportadas.

#### Como gerar o apk utilizando o EAS local
`eas build -p android --profile preview --local`

```json
{
  "cli": {
    "version": ">= 16.4.1",
    "appVersionSource": "remote"
  },
  "build": {
    "preview": {
      "android": {
        "buildType": "apk"
      },
      "env": {
        "EXPO_PUBLIC_WEATHER_APP_ID": "b3125618fd66303f44adebd1f7acd23f"
      }
    }
  }
}
````

#### Como gerar o apk utilizando o cloud do EAS
Você pode acompanhar o build pela plataforma do Expo.

`eas build -p android --profile preview`

```json
{
  "cli": {
    "version": ">= 16.4.1",
    "appVersionSource": "remote"
  },
  "build": {
    "preview": {
      "android": {
        "distribution": "internal"
      },
      "env": {
        "EXPO_PUBLIC_WEATHER_APP_ID": "b3125618fd66303f44adebd1f7acd23f"
      }
    }
  }
}

```

### Como gerar apk (.aab) para produção EAS

`eas build -p android --profile production`

```json
{
  "cli": {
    "version": ">= 16.4.1",
    "appVersionSource": "remote"
  },
  "build": {
    "preview": {
      "android": {
        "distribution": "internal"
      },
      "env": {
        "EXPO_PUBLIC_WEATHER_APP_ID": "b3125618fd66303f44adebd1f7acd23f"
      }
    },
    "production": {
      "env": {
        "EXPO_PUBLIC_WEATHER_APP_ID": "b3125618fd66303f44adebd1f7acd23f"
      }
    }
  }
}
```