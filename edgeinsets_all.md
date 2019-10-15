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
        title: Text('Demo EdgeInsets.all()'),
      ),
      body: Row(
        children: <Widget> [ 
          Container (
            color: Colors.lightBlue,
            margin: const EdgeInsets.all(20.0),
            padding: const EdgeInsets.all(5.0),        
            child: RaisedButton(
              child: Text('Button 1'),
              onPressed: () {}
            ),
          ),
          Container (
            margin: const EdgeInsets.all(5.0),
            padding: const EdgeInsets.all(10.0),
            decoration: BoxDecoration(
              border: Border.all(
                width: 5.0,
                color: Colors.red,
              )
            ),            
            child: RaisedButton(
              child: Text('Button 2'),
              onPressed: () {}
            ),
          ),
          Container (
            color: Colors.lightBlue,
            margin: const EdgeInsets.all(20.0),
            padding: const EdgeInsets.all(5.0),        
            child: RaisedButton(
              child: Text('Button 3'),
              onPressed: () {}
            ),
          ),
        ],
      ),
    );
  }
}


</pre>
