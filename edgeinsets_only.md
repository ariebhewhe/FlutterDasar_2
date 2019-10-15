<pre>
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
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
        title: Text('Demo EdgeInsets.only()'),
      ),
      body: Row(
        children: <Widget> [ 
          Expanded(
            child: Container (
              color: Colors.lightBlue,
              margin: const EdgeInsets.only(top: 50.0),
              padding: const EdgeInsets.only(left: 70.0, right: 10.0),        
              child: RaisedButton(
                child: Text('Button'),
                onPressed: () {}
              ),
            ),
          ),
        ],
      ),
    );
  }
}


</pre>
