import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: RichTextDemo(),
 );
 }
}
class RichTextDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('RichText Example')),
 body: Center(
 child: RichText(
 text: TextSpan(
 children: <TextSpan>[
 TextSpan(
 text: 'Hello, ',
 style: TextStyle(color: Colors.black, fontSize: 20),
 ),
 TextSpan(
 text: 'Flutter!',
 style: TextStyle(color: Colors.blue, fontSize: 30, 
fontWeight: FontWeight.bold),
 ),
 TextSpan(
 text: ' Welcome to RichText widget.',
 style: TextStyle(color: Colors.green, fontSize: 18),
 ),
 ],
 ),
 ),
 ),
 );
 }
}
