# ODC-THEMES
Themes for OpenSID

Ada beberapa hal yang perlu di buat untu mendukung template ini (Optional) :
- ubah artikel per-page menjadi 6 di "donjo-app/models/first-artikel_m.php" --> lakukan pengeditan pada baris 52 dari $cfg['per_page'] = 8; jadi $cfg['per_page'] = 6;
- tambah kode :
		if (is_file('desa/themes/odc/layouts/kategori.php')) {
			$this->set_template('layouts/kategori.php');
		}
  dibawah kode $this->_get_common_data($data); pada function function kategori($kat=0,$p=1){ di donjo-app/controllers/First.php,	ini digunakan untuk memisahkan tampilan kategori dengan menu utama artikel
  
  Demo Tema ODC di https://odc.orapakat.com
