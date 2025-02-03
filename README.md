
This project is just for fun and to fill my free time. so please try it and have fun.

---

# Indonesia Script Language

indonesia script language adalah sebuah bahasa pemrograman baru, yang modern dan mudah di pelajari karena menggunakan bahasa indonesia. untuk menggunakan nya pun sederhana tidak perlu pengalaman coding 

## Instalation & Run
PASTIKAN KAMU SUDAH MENGINSTALL NODE JS

Install from npm
```bash
npm install -g indonesia-script-language
```

### Run

run isl script using `isl` command

```bash
isl app.isl
```



## Example 

Example : 

```
sementara umur adalah 18
tampilkan "Umur lu " + umur
kalau umur lebih gede 17
  tampilkan "kamu remaja"
  sementara umurku adalah umur + 10
  tampilkan "kalau aku umurnya " + umurku
  kalau umurku lebih gede 30
    tampilkan "aku lebih tua"
  berhenti
kalaugak
  tampilkan "dasar bocil"
berhenti
tampilkan "kaburrr"
```

```
sementara jumlah adalah 10
tampilkan "Jumlah: " + jumlah

yang mana jumlah adalah 11
tampilkan "Jumlah: " + jumlah

sementara isHidup adalah benar
tampilkan "is hidup :" + isHidup

untuk i hingga 10
  kalau i lebih gede 3
    tampilkan "loop ke " + i
  berhenti
berhenti
```

### Command

### Variable

Assign variable
```
sementara foo adalah "hello world"
// let foo = "hello world"

seriously foo adalah 123
// const foo = 123
```

Reassign variable
```
yang mana foo adalah "hello world 2"
// foo = "hello world 2"
```

**Boolean**

```
sementara foo adalah benar
// let foo = true

sementara foo adalah benar
// let foo = true

sementara foo adalah salah
// let foo = false
```

### Print / Console.log
```
tampilkan "Hello world"
// console.log("Hello world")

tampilkan foo
// console.log(foo)
```


### Condition

```
kalau foo adalah "Hello world"
  tampilkan "its hello world"
berhenti

// transform to
if(foo == "Hello world"){
  console.log("its hello world")
}
```

```
kalau foo lebih gede 3
  tampilkan "its bigger than 3"
seandainya foo adalah 3
  tampilkan "foo is 3"
kalaugak
  tampilkan "its smaller than 3"
berhenti

// transform to
if(foo > 3){
  console.log("its bigger than 3")
} else if (foo == 3) {
  console.log("foo is 3")
} else {
  console.log("its smaller than 3")
}
```

Comparison : 
- `adalah`: ' == ',
- `gak`: ' != ',
- `lebih gede`: ' > ',
- `lebih kecil`: ' < ',
- `lebih gede sama dengan`: ' >= ',
- `lebih kecil sama dengan`: ' <= '

### Loop

#### **`For` loop**:
```
untuk i hingga 10
  kalau i lebih gede 3
    tampilkan "loop ke " + i
  berhenti
berhenti

// transform to
for (let i = 0; i < 10; i++) {
  if (i > 3){
    console.log("loop ke " + i);
  }
}
```

#### **`For of` loop**:
```
untuk semua foo dari bar
  tampilkan foo
berhenti

// transform to
for (const foo of bar) {
  console.log(foo);
}
```

#### **`break`** and **`continue`**:
```
stop
// break;

skip
// continue;
```

### Function
```
fungsi my_story
    sementara umur adalah 21
    tampilkan "Umur lu " + umur
selesai

call my_story

fungsi fungsi_param_banyak a b c
    tampilkan "a: " + a
    tampilkan "b: " + b
    tampilkan "c: " + c
selesai

call fungsi_param_banyak 3 4 5
```

### Async Function
```
asinksi fungsi my_story
    sementara umur adalah 21
    tampilkan "Umur lu " + umur
selesai

call my_story

fungsi fungsi_param_banyak a b c
    tampilkan "a: " + a
    tampilkan "b: " + b
    tampilkan "c: " + c
selesai

call fungsi_param_banyak 3 4 5
```

### Try Catch & Exception
```
coba
  tampilkan "Something wrong"
  gagal "Error message"
tangkap
  tampilkan "Catch error"
akhirnya
  tampilkan "finish finally"
berhenti


// transform to
try {
  console.log("Something wrong");
  throw new Error("Error message");
} catch {
  console.log("Catch error");
} finally {
  console.log("finish finally");
} 
```


### Disclaimer

Project ini hanya untuk bersenang senang tidak ada niatan untuk melukai atau pun menjelekkan pihak lain


# indonesia-script-language
