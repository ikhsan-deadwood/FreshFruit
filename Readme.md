FRESH FRUIT

Freash Fruit merupakan program yang digunakan untuk menambahkan buah-buahan kedalam keranjang, disertai menampilkan gambar.

Fungsi

    Users dapat menekan button Add untuk menambahkan buah/fruit
    Users dapat menghapus nama buah yang sudah tampil dikeranjang dengan menekan button DELETE.

Cara Kerja Program?

Pada Method Fruit.cs itu merupakan Logic View yang digunakan untuk menampilkan nama buah pada listbox. berikut merupakan source codenya
```
 public string name { get; set; }

        public Fruit(string name)
        {
            this.name = name;
        }
        public string getName()
        {
            return this.name;
        }
```
Berikut merupakan source code pada MainWindow.xaml.cs
```
 private void Button1_Click(object sender, RoutedEventArgs e)
        {
            Fruit anggur = new Fruit("Anggur");
            Ikhsan.addFruit(anggur);
        }

        private void Button2_Click(object sender, RoutedEventArgs e)
        {
            Fruit apel = new Fruit("Apel");
            Ikhsan.addFruit(apel);
        }

        private void Button3_Click(object sender, RoutedEventArgs e)
        {
            Fruit pisang = new Fruit("Pisang");
            Ikhsan.addFruit(pisang);
        }

        private void Button4_Click(object sender, RoutedEventArgs e)
        {
            Fruit jeruk = new Fruit("Jeruk");
            Ikhsan.addFruit(jeruk);
        }
```