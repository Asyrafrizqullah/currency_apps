# currency_apps
Membuat aplikasi nilai mata uang amerika serikat dalam bentuk Rupiah menggunakan C#
pertanyaan
1.Review kembali percobaan 1 sampai dengan 3 dengan menjawab pertanyaan-pertanyaan pada latihan tersebut.
2.Mengapa perlu membuat class CurrencyController.cs pada percobaan 4 ?
3.Jelaskan kegunaan method isAllowed pada percobaan 4!
4.Jelaskan secara singkat mengenai Regex pada percobaan 4!
5.Buatlah class diagramnya pada percobaan 4! 
jawaban
1.sudah
2.membuat class currencycontroller.cs pada percobaan ke empat, untuk mengubah nilai pada mata uang US yang dimana nilai 1 dollar us di ubah ke Rupiah menjadi Rp.1500 merubahnya menjadi variabel.
class CurrencyController
    {
        public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);// mengubah nilai nominal
            var result = nominalDouble * 15000;// satuan us dollar amerika menjadi Rp.1500
            return Convert.ToString(result);
        }

        public Boolean isAllowed(string nominal)
        {
            Regex regex = new Regex("[^0-9.-]+");//matching mempertemukan nilai mata uang yang di convert
            return !regex.IsMatch(nominal);
        }
    }
3. untuk memanggil sebuah class method agar dapat di running
4.Regex merupakan sebuah teks (string) yang mendefinisikan sebuah pola pencarian sehingga dapat membantu kita untuk melakukan matching (pencocokan), locate (pencarian), dan manipulasi teks.
5.jawaban ke lima saya kirim dalam format jpg.
