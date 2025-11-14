---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Pàgina inicial
---

#Benvingut al meu lloc Jekyll

Aquesta és una pàgina creada amb **Markdown avançat**.
Feta pel **Jaume**

---

<!-- Menú de navegació -->
<nav style="background-color:#333; padding:10px; text-align:center;">
  <a href="/" style="color:white; margin:0 15px; text-decoration:none;">Inici</a>
  <a href="/about/" style="color:white; margin:0 15px; text-decoration:none;">Sobre Nosaltres</a>
  <a href="/serveis/" style="color:white; margin:0 15px; text-decoration:none;">Serveis</a>
</nav>

---

## Taula

Aquí he posat una taula:

| Nom       | Tipus              | Notes            |
|-----------|--------------------|------------------|
| Jekyll    | Generador web      | Ràpid i senzill  |
| Markdown  | Llenguatge lleuger | Facil d'aprendre |

---

## Imatge

https://www.bing.com/images/search?view=detailV2&ccid=km1rfSJL&id=1FA8F859D6F47B88290704D61A04BCFFEE33FE36&thid=OIF.Oqtow2n6jg6D1Zd%2fTcq5BQ&mediaurl=https%3a%2f%2finfodelestero.com%2fwp-content%2fuploads%2f2025%2f11%2fimage-56-1146x645.jpg&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.926d6b7d224be855c93c4a84e48d63db%3frik%3d%26pid%3dImgRaw%26r%3d0&exph=645&expw=1146&q=foto+messi+camp+nou&FORM=IRPRST&ck=3AAB68C369FA8E0E83D5977F4DCAB905&selectedIndex=1&itb=0


---

##Bloc de codi delimitat.
##Generador de hashes.

```
{

import hashlib

# Demanem la contrasenya
password = input("Escriu la contrasenya: ")

# Mostrem el menú
print("Escull quin algoritme vols utilitzar:")
print("1. MD5")
print("2. SHA1")
print("3. SHA256")
print("4. SHA384")
print("5. SHA512")

menu = input("Opió: ")

# Convertim la contrasenya a bytes (necessari per hashlib)
pw_bytes = password.encode()

# Fem el hash segons l’opció
if menu == "1":
    hash_result = hashlib.md5(pw_bytes).hexdigest()
    alg = "MD5"
    # Per guardar el hash al fitger
    with open("md5.txt", "w") as file: 
        file.write(hash_result)

elif menu == "2":
    hash_result = hashlib.sha1(pw_bytes).hexdigest()
    alg = "SHA1"
    # Per guardar el hash al fitger
    with open("sha1.txt", "w") as file: 
        file.write(hash_result)

elif menu == "3":
    hash_result = hashlib.sha256(pw_bytes).hexdigest()
    alg = "SHA256"
    # Per guardar el hash al fitger
    with open("sha256.txt", "w") as file: 
        file.write(hash_result)

elif menu == "4":
    hash_result = hashlib.sha3_384(pw_bytes).hexdigest()
    alg = "SHA384"
    with open("sha384.txt", "w") as file:
        file.write(hash_result)
elif menu == "5":
    hash_result = hashlib.sha512(pw_bytes).hexdigest()
    alg = "SHA512"
    with open("sha512.txt", "w") as file:
        file.write(hash_result)

else:
    print("Opció no vàlida.")
    exit()

# Mostrem el resultat
print("\nAquesta és la contrasenya original:")
print(password)
print("------------------------------")
print(f"Aquest és el hash generat amb {alg}:")
print(hash_result)
print(f"S'ha guardat al fitxer {alg}.txt")

}
```

---

##Text taxat.

Fidel Castro.
~~Solo que ahora libertad quiere decir algo más todavía: libertad quiere decir patria.~~
La dictadura militar a Cuba ha durat més de 66 anys, començant des del triomf de la Revolució liderada per Fidel Castro en 1959. 
Des de llavors, Cuba ha estat sota un règim autoritari que ha mantingut un control absolut sobre tots els aspectes de la vida política, 
econòmica i social de totes les persones.

Che Guevara.
~~Fusilamientos, sí, hemos fusilado, fusilamos y seguiremos fusilando mientras sea necesario.~~
Aquesta declaració va ser pronunciada en un discurs davant les Nacions Unides en 1964, 
on Guevara va admetre que la revolució cubana havia dut a terme afusellaments com a 
part de la seva lluita per la llibertat i la justícia.
