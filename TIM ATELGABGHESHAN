program SistemPenggajian;
uses crt;

type
    Karyawan = record //penggunaann record untuk menciptakan field, agar mudah untuk mengorganisir data
        nama: string;
        jamKerja: integer;
        masaKerja: integer;
        gajiPokok: real;
        totalGaji: real;
    end;

var
    dataKaryawan: array[1..100] of Karyawan; //penggunaan array agar data dapat disimpan berurutan
    jumlahKaryawan: integer;
    f: text;

function hitungBonus(masaKerja: integer): real;
begin
    if masaKerja <= 1 then
        hitungBonus := 0.05  // 5% untuk masa kerja <= 1 tahun
    else
        hitungBonus := 0.05 + hitungBonus(masaKerja - 1) * 1.5;  // Bonus bertambah 1.5x setiap tahun
end;
