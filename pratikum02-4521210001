package main

import (
	"fmt"
)

type Mahasiswa struct {
	Nama    string
	Npm     string
	Jurusan string
}

func main() {
	// Menyimpan data mahasiswa dalam map
	mahasiswa := map[string]Mahasiswa{
		"4521210004": {Nama: "Danu", Npm: "4521210004", Jurusan: "Teknik Informatika"},
		"4521210001": {Nama: "Alam", Npm: "4521210001", Jurusan: "Teknik Informatika"},
	}

	// Menampilkan daftar nama mahasiswa dengan perulangan
	fmt.Println("Daftar nama mahasiswa:")
	for _, mhs := range mahasiswa {
		fmt.Println("-", mhs.Nama)
	}

	// Mencari data mahasiswa berdasarkan NPM
	fmt.Println("\nCari data mahasiswa berdasarkan NPM:")
	var npm string
	fmt.Scanln(&npm)

	mhs, ok := mahasiswa[npm]
	if ok {
		fmt.Printf("Nama: %s\nNPM: %s\nJurusan: %s\n", mhs.Nama, mhs.Npm, mhs.Jurusan)
	} else {
		fmt.Println("Mahasiswa dengan NPM", npm, "tidak ditemukan.")
	}
}
