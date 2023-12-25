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

Warna: Rumput Hijau
# Analysis : User Story

|Sebagai|Saya ingin bisa|Sehingga|Prioritas|
|-----|-----|-----|-----|
|Pemain|Memakan Makanan|Ular Menjadi Panjang|⭐⭐⭐⭐⭐|
|Pemain|Melewati Rintangan|Skor Bertambah|⭐⭐⭐⭐⭐|
|Pemain|Memilih Berbagai Ular|Mempunyai Keunikan Masing-Masing|⭐⭐⭐⭐|



# Desain user interface
![WhatsApp Image 2023-12-25 at 19 21 19](https://github.com/Davidmhvk/P-Daspro/assets/144786308/8f229216-6009-4754-ab78-1de4f4f310f4)


# Flow chart dari algoritma
![FlowChartSnake](https://github.com/Davidmhvk/P-Daspro/assets/144786308/5f323df9-8c53-4c22-90b2-f7172de1a56f)


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
