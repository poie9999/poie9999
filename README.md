import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: MyHomePage(),
    );
  }
}

class MyHomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Identitas Mahasiswa'),
      ),
      body: Center(
        child: Column(
          children: <Widget>[
            Container(
              height: 170,
              width: 300,
              padding: EdgeInsets.all(10),
              alignment: Alignment.topCenter,
              decoration: BoxDecoration(
                border: Border.all(width: 5),
              ),
              child: Text(
                'NIM: 22.240.0034\nNama: M.Islakhul Fani\nKelas: 3P41\nJenjang: S1\nProgdi: Teknik Informatika\nKonsentrasi: Teknik Informatika',
                style: TextStyle(
                  fontSize: 18,
                ),
                textAlign: TextAlign.left,
              ),
            ),
          ],
        ),
      ),
    );
  }
}
