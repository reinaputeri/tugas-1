# tugas-1
#include <iostream>
using namespace std;

int main () {
    
    //kamus
    
    int ember_3 = 3;
    int ember_5 = 5;
    int ember_4 = 4;
    
    
    cout << "Sistem Pengisian Ember\nPilihlah 6 langkah dibawah untuk mengisi ember 4L sampai penuh!\n\n";
    cout << "1. Isi ember 3L\n";
    cout << "2. isi ember 5L\n";
    cout << "3. Kosongkan ember 3L\n";
    cout << "4. Kosongkan ember 5L\n";
    cout << "5. Tuang ember 3L ke ember 5L\n";
    cout << "6. Tuang ember 5L ke ember 3L\n"; 
    
    //algoritma
    
    int nomor_instruksi;
    int sum_ember_3;
    int sum_ember_5;
    cout << "Masukkan nomor instruksi : \n"; //input data
    cin >> nomor_instruksi;
    
    while (sum_ember_3 != 4 || sum_ember_5 != 4){
    	if (nomor_instruksi = 1){
    		int sum_ember_3 = ember_3 - 3 ;
    		cout << "ember 3 = "<< sum_ember_3 <<"L\n ember 5 = "<<ember_5;
    	}        
    	else if (nomor_instruksi = 2) {
        	int sum_ember_5 = ember_5 - 5 ;
            cout << "ember 3 = "<< ember_3 << "L\n ember 5 = "<< sum_ember_5;
    	}
    	else if (nomor_instruksi = 3) {
        	int sum_ember_3 = 0;
            cout << "ember 3 = "<< sum_ember_3 << "L\n ember 5 = "<< sum_ember_5; 
    	}
    	else if (nomor_instruksi = 4) {
        	int sum_ember_5 = 0;
            cout << "ember 3 = "<< sum_ember_3 << "L\n ember 5 = "<< sum_ember_5;
    	}
    	else if (nomor_instruksi = 5) {
        	int sum_ember_3 = ember_3 + (ember_5-3);
            int sum_ember_5 = ember_5 + sum_ember_3;
            cout <<"ember 3 = "<< sum_ember_3 << "L\n ember 5 = "<< sum_ember_5;
    	}
    	else if (nomor_instruksi = 6) {
        	int sum_ember_3 = ember_3 + (ember_5-3);
            int sum_ember_5 = ember_5 + sum_ember_3;
            cout <<"ember 3 = "<< sum_ember_3 << "L\n ember 5 = "<< sum_ember_5;
    	}
    	else { //input nomor <1 atau >6
    		cout << "Masukkan kembali nomor instruksi";
   		}
    return 0;
    }
}
