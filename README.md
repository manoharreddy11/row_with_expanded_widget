import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Row with Expanded Widgets Example'),
        ),
        body: Center(
          child: Row(
            children: [
              Expanded(
                flex: 2,
                child: Container(
                  color: Colors.blue,
                  height: 100,
                  child: Center(child: Text('Left')),
                ),
              ),
              Expanded(
                flex: 1,
                child: Container(
                  color: Colors.green,
                  height: 100,
                  child: Center(child: Text('Right')),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
