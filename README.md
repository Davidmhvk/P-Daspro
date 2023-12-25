# Latar Belakang Membuat game
Snake Cobs merupakan permainan yang sederhana namun menghibur. permainan ini melibatkan ular yang terus tumbuh saat memakan objek (biasanya diberi representasi sebagai makanan) di dalam area terbatas. Tujuan utama pemain adalah menghindari benturan dengan batas atau tubuh ular sendiri. Keseruan game ini terletak pada tantangan untuk mempertahankan panjang ular seiring berjalannya waktu.
# Deskripsi dan alur cerita dari game
Sebuah Game yang didalamnya terdapat seorang player yang menjadi ular yang dimana tugas player itu adalah mencari makan untuk ular tersebut dan menghindari rintangan-rintangan yang ada didalam game tersebut.Apabila ular/player memakan makanan tersebut maka ular akan menjadi panjang dan akan menampilkan skor dari ular tersebut, Apabila ular/player terkena rintangan maka ular itu akan berkurang skornya dan lama kelamaan akan mati.
# Analysis : Branding
Merk: Snake Cobs

Tagline: Bimbinglah ular sebaik mungkin

Campaign: Bagaimana membuat game yang membuat penggunanya senang dengan tantangan dan adrenalin

Target user:

Usia 4+

Seorang yang antusias memecahkan rekor

Seorang yang senang mengacu adrenalin

Seorang yang berani mengambil risiko

Seorang yang ingin bermain game yang menantang

User experience theme:

Mudah

Sederhana

Menyenangkan

Warna: nuansa pagi hari
# Analysis : User Story

|Sebagai|Saya ingin bisa|Sehingga|Prioritas|
|-----|-----|-----|-----|
|Pemain|Berjalan kaki ke kampus|Bisa berjalan kaki kekampus|⭐⭐⭐⭐⭐|
|Pemain|Naik bus/angkot ke kampus|Bisa naik bus/angkot kekampus|⭐⭐⭐⭐⭐|
|Pemain|Mengendarai motor ke kampus|Bisa mengendarai motor kekampus|⭐⭐⭐⭐⭐|
|Pemain|Melihat petunjuk atau tujuan saat menjalani perjalanan|Bisa menampilkan secara jelas untuk membimbing pemain|⭐⭐⭐|
|Pemain|Mendapatkan tantangan atau misi baru selama perjalanan|Bisa memainkan game dengan lebih seru |⭐⭐⭐⭐⭐|
|Pemain|Mendapatkan imbalan atau poin setelah menyelesaikan setiap perjalanan|Bisa mendapatkan keuntungan dalam permainan|⭐⭐⭐⭐|
|Pemain|Dapat menghentikan atau menyimpan perjalanan saat saya keluar dari permainan|Bisa menyimpan perjalanan dan melanjutkannya di sesi berikutnya|⭐⭐⭐⭐|
|Pemain|Memiliki pilihan untuk mengulang perjalanan atau memulai perjalanan baru|Bisa memberikan pengalaman yang berbeda|⭐⭐⭐⭐|
|Pemain|Melihat dan mengelola pencapaian selama permainan|Bisa melihat pencapaian yang telah dicapai selama permainan|⭐⭐⭐|
|Pemain|Melihat skor atau poin saya saat bermain|Bisa melihat perolehan poin mereka di menu atau antarmuka lainnya|⭐⭐⭐⭐|
|Pemain|Memilih karakter sebelum memulai permainan|Bisa memilih karakter dari beberapa opsi yang tersedia|⭐⭐⭐|
|Pemain|Memulai perjalanan baru untuk mengeksplorasi permainan|Bisa memulai perjalanan baru dari awal|⭐⭐⭐⭐|
|Pemain|Merasakan perubahan cuaca (seperti hujan)|Bisa mempengaruhi tantangan dan pengalaman permainan|⭐⭐⭐⭐|



# Desain user interface
![WhatsApp Image 2023-12-18 at 11 48 51_a76bed23](https://github.com/elsasitimariyam/TugasUTSPDP/assets/144762238/8786e563-2318-4773-b375-9a65cfac8179)

# Flow chart dari algoritma
![Flowchart game-Page-1](https://github.com/elsasitimariyam/TugasUTSPDP/assets/144762238/2671a9a8-cb44-4e1e-972e-90de63583598)

# Link demo game di Youtube
# Link folder kode pemrograman dari game
[game PDP.txt](https://github.com/elsasitimariyam/TugasUTSPDP/files/13698307/game.PDP.txt)

# Bagaimana konsep variable, data type dan operator pada bahasa pemrograman digunakan dalam pembuatan game ini ?
Dalam pembuatan game dengan bahasa pemrograman Java, konsep variabel, tipe data, dan operator sangat penting untuk mengelola data dan melakukan operasi yang diperlukan. Berikut ini salah satu cara konsep yang saya gunakan dalam pembuatan game

variabel 

	private int ularX, ularY;

tipe data

	private int ularX, ularY;

operator

	 if (ularX < 0) {
		ularX = KOTAK_SIZE - 1;
  
# Bagaimana konsep boolean dan conditions pada bahasa pemrograman digunakan dalam pembuatan game ini ?
Konsep kondisi (conditions) dalam bahasa pemrograman Java sangat penting dalam pembuatan game karena memungkinkan kontrol alur program berdasarkan keadaan atau situasi tertentu. Salah satu cara konsep kondisi yang saya gunakan dalam pembuatan game

	if (ularX == MAKANANX && ularY == MAKANANY) {
        	MAKANAN();
    	}
        
        if (ularX < 0) {
        ularX = KOTAK_SIZE - 1;
	} else if (ularX >= KOTAK_SIZE) {
        ularX = 0;
    	}

    	if (ularY < 0) {
        	ularY = KOTAK_SIZE - 1;
	} else if (ularY >= KOTAK_SIZE) {
        ularY = 0;
	}
 
# Bagaimana konsep looping dan array pada bahasa pemrograman digunakan dalam pembuatan game ini ?
Array

	private char[][] grid;

 	public void initGame() {
   	 	for (int i = 0; i < KOTAK_SIZE; i++) {
        		for (int j = 0; j < KOTAK_SIZE; j++) {
            		grid[i][j] = EMPTY_CELL;
       		 	}
   		 }

  		ularX = KOTAK_SIZE / 2;
   		ularY = KOTAK_SIZE / 2;
  		grid[ularX][ularY] = ULAR_CELL;

   		MAKANAN();
	}

 Looping

	public static void main(String[] args) {
    		Scanner scanner = new Scanner(System.in);
   		 UlarGame game = new UlarGame();

    		while (true) {
       			game.displayGrid();
        		System.out.print("Gunakan tombol (w/a/s/d) atau 'q' untuk keluar dari game: ");
        		char direction = scanner.next().charAt(0);

        		if (direction == 'q') {
            		System.out.println("Terima kasih sudah bermain!");
           		break;
        		}

			game.move(direction);
    		}

    	scanner.close();
	}

# Bagaimana konsep method pada bahasa pemrograman digunakan dalam pembuatan game ini ?
Konsep metode (method) dalam bahasa pemrograman Java sangat penting dalam pembuatan game karena metode digunakan untuk mengorganisir dan mendefinisikan perilaku atau fungsi-fungsi tertentu. Salah satu cara konsep method yang saya gunakan dalam pembuatan game 

	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		UlarGame game = new UlarGame();
    
# Bagaimana konsep class pada bahasa pemrograman digunakan dalam pembuatan game ini ?
Konsep class dalam bahasa pemrograman Java sangat penting dalam pengembangan game. Class digunakan untuk mengorganisir kode secara objek-oriented, memungkinkan pembuatan objek dan pengelolaan fitur-fitur yang terkait dengan entitas tertentu dalam permainan. salah satu cara konsep class yang saya gunakan dalam pembuatan game Java

	public class UlarGame {

# Jelaskan algoritma buatan sendiri yang digunakan pada pembuatan game ini !
