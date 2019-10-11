# syntak 
<pre>
Row   : <Widget>[
  // komponen 1,
  // komponen 2,
  // komponen 3,
  //.....
  ]
  </pre>
mainAxisAlignment untuk menentukan posisi komponent pada layar (MainAxisAlignment.center,MainAxisAlignment.start,: MainAxisAlignment.end)

# Membuat Tampilan Baris

<pre> 
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Demo Flutter',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: Home(),
    );
  }
}

class Home extends StatelessWidget {  
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Demo Row'),
      ),
      body: Center(
        child: Row(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            RaisedButton(
              child: Text('Button 1'),
              onPressed: () {},
            ),
            Container(width: 10),
            RaisedButton(
              child: Text('Button 2'),
              onPressed: () {},
            ),
            Container(width: 10),
            RaisedButton(
              child: Text('Button 3'),
              onPressed: () {},
            ),
            Container(width: 10),
            RaisedButton(
              child: Text('Button 4'),
              onPressed: () {},
            ),
            
          ],
        ),
      ),      
    );
  }
}


</pre>
