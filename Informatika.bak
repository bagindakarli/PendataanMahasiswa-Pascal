Program Informatika;
uses crt;
type tipemhs = record
        nama:string;
        nim:integer;
        jk:char;
        nilai:integer;
end;

var
        mhs:array[1..30] of tipemhs;
        i,j,m,nasli,max,min:integer;
        nama:string;
        nim:integer;

function rata(x:integer):real;
var
        avg:real;
begin
        avg:=x/m;
        rata:=avg;
end;

procedure awal;forward;

procedure tambah;
begin
end;

procedure edit;
var
        nimsearch:integer;
        ubahfix:char;
begin
clrscr;
                        writeln;
                        writeln('=======================');
                        writeln(' PENCARIAN MAHASISWA/I');
                        writeln('=======================');
                        writeln;
                        write('Masukkan NIM Mahasiswa/i : ');readln(nimsearch);
                        for i:=1 to m do
                                begin
                                        if (nimsearch=mhs[i].nim) then
                                                begin
                                                        writeln;
                                                        writeln('[1] Nama          : ',mhs[i].nama);
                                                        writeln('[2] Jenis Kelamin : ',mhs[i].jk);
                                                        writeln('[3] Nilai         : ',mhs[i].nilai);
                                                        writeln;
                                                        write('Pilih nomor yang ingin diubah datanya.. ');readln(ubahfix);
                                                        writeln;
                                                        case ubahfix of
                                                                '1':    begin
                                                                                write('Nama : ');readln(mhs[i].nama);
                                                                                writeln('Data berhasil diubah');readln;
                                                                        end;
                                                                '2':    begin
                                                                                write('Jenis Kelamin [L/P] : ');readln(mhs[i].jk);
                                                                                writeln('Data berhasil diubah');readln;
                                                                        end;
                                                                '3':    begin
                                                                                write('Nilai : ');readln(mhs[i].nilai);
                                                                                if j=1 then
                                                                                        begin
                                                                                                max:=mhs[j].nilai;
                                                                                                min:=mhs[j].nilai;
                                                                                        end
                                                                                else
                                                                                        begin
                                                                                                if mhs[j].nilai > max then
                                                                                                        begin
                                                                                                                max:=mhs[j].nilai;
                                                                                                        end
                                                                                                else if mhs[j].nilai < min then
                                                                                                        begin
                                                                                                                min:=mhs[j].nilai;
                                                                                                        end;
                                                                                        end;
                                                                                writeln('Data berhasil diubah.');readln;
                                                                        end;
                                                        end;
                                                awal;
                                                end
                                        else
                                                begin
                                                        writeln('Loading..');readln;
                                                end;

                                end;

end;

procedure tampil;
begin
clrscr;
writeln('====================');
writeln('  DATA MAHASISWA/I  ');
writeln('====================');
writeln;
for i:=1 to m do
        begin
                writeln('NIM           : ',mhs[i].nim);
                writeln('Nama          : ',mhs[i].nama);
                writeln('Jenis Kelamin : ',mhs[i].jk);
                writeln('Nilai         : ',mhs[i].nilai);
                writeln;
        end;
readln;
awal;
end;

procedure datasiswa;
var
        jmhs,jkls,totmhs,n,totnilai:integer;
        ubah,ubahfix:char;
        nimsearch:integer;
begin
        clrscr;
        writeln('=============================');
        writeln('   TEKNIK INFORMATIKA 2017   ');
        writeln('=============================');
        writeln;
        writeln('        ------------');
        writeln('         DATA SISWA');
        writeln('        ------------');
        writeln;
        write('Masukkan Jumlah Kelas : ');readln(jkls);
        writeln;
        m:=0;
        nasli:=0;
        max:=0;
        for i:=1 to jkls do
                begin
                        write('     Masukkan Jumlah Mahasiswa/i IF 41-0',i,' : ');readln(jmhs);
                        totmhs:=jmhs+m;
                        m:=totmhs;
                        writeln;
                        n:=0;
                        for j:=1 to jmhs do
                                begin
                                        writeln('          -------------------');
                                        writeln('           MAHASISWA/I ke-',j);
                                        writeln('          -------------------');
                                        writeln;
                                        write('          Nama                : ');readln(mhs[j].nama);
                                        write('          NIM                 : ');readln(mhs[j].nim);
                                        write('          Jenis Kelamin (L/P) : ');readln(mhs[j].jk);
                                        write('          Nilai               : ');readln(mhs[j].nilai);
                                        writeln;
                                        totnilai:=mhs[j].nilai+n;
                                        n:=totnilai;
                                        if j=1 then
                                                begin
                                                        max:=mhs[j].nilai;
                                                        min:=mhs[j].nilai;
                                                end
                                        else
                                                begin
                                                        if mhs[j].nilai > max then
                                                                begin
                                                                        max:=mhs[j].nilai;
                                                                end
                                                        else if mhs[j].nilai < min then
                                                                begin
                                                                        min:=mhs[j].nilai;
                                                                end;
                                                end;
                                end;
                        nasli:=nasli+n;
                end;
        writeln;
        write('Data Sudah Tersimpan.');
        readln;
        awal;
end;

procedure awal;
var
        menu:char;
begin
        clrscr;
        writeln('=============================');
        writeln('---TEKNIK INFORMATIKA 2017---');
        writeln('=============================');
        writeln;
        writeln('[1] DATA SISWA');
        writeln('[2] STATISTIK');
        writeln('[3] EDIT DATA MAHASISWA');
        writeln('[4] TAMBAH DATA MAHASISWA');
        writeln('[5] TAMPILKAN SEMUA');
        writeln;
        writeln('[0] EXIT');
        writeln;
        write('Silakan pilih menu... ');readln(menu);
        if menu = '1' then
                begin
                        datasiswa;
                end
        else if menu = '2' then
                begin
                        clrscr;
                        writeln('=============================');
                        writeln('   TEKNIK INFORMATIKA 2017   ');
                        writeln('=============================');
                        writeln;
                        writeln('        -----------');
                        writeln('         STATISTIK');
                        writeln('        -----------');
                        writeln;
                        writeln('Total Mahasiswa/i Teknik Informatika 2017       : ',m);writeln;
                        writeln('Total Nilai Mahasiswa/i Teknik Informatika 2017 : ',nasli);writeln;
                        writeln('Rata-Rata                                       : ',rata(nasli));writeln;
                        writeln('Nilai Tertinggi                                 : ',max);
                        {writeln('    Nama : ',nama,'                  ');
                        writeln('    NIM  : ',nim,'                  ');   }
                        writeln;
                        writeln('Nilai Terendah                                  : ',min);
                        {writeln('    Nama : ',nama,'                  ');
                        writeln('    NIM  : ',nim,'                  ');   }
                        writeln;
                        readln;
                awal;
                end
        else if menu = '3' then
                begin
                        edit;
                end
        else if menu = '4' then
                begin
                        tambah;
                end
        else if menu = '5' then
                begin
                        tampil;
                end
        else if menu = '0' then
                begin
                        exit;
                end
        else
                begin
                        writeln('Pilih menu dengan benar.');readln;
                        awal;
                end;
end;



begin
{COPYRIGHT BAGINDA ACHMAD KARLI NOVEMBER 17}
clrscr;
awal;
end.


