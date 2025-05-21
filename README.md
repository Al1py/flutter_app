# flutter_app
training flutter
import 'package:flutter/material.dart';
void main(){
  runApp(MyApp());
}
class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return  MaterialApp(
      home: SafeArea(
          child:Scaffold(
            backgroundColor: Colors.white,
            appBar: AppBar(
              title: Text("ALI STORE",style: TextStyle(color: Colors.white,fontWeight: FontWeight.bold),),
              centerTitle: true,
              backgroundColor: Colors.black,
            ),
            body: ListView(
              children: [
                Padding(
                  padding: const EdgeInsets.all(12.0),
                  child: Row(
                    mainAxisAlignment: MainAxisAlignment.spaceBetween,
                    mainAxisSize: MainAxisSize.max,
                    children: [
                      Icon(Icons.menu_outlined,color: Colors.black,size: 30,),
                      Row(
                        children: [
                          Icon(Icons.shopping_bag_outlined,color: Colors.black,size: 30,),
                          SizedBox(width: 10,),
                          Icon(Icons.favorite_border_outlined,color: Colors.black,size: 30,),
                          SizedBox(width: 10,),
                        ]
                      )
                    ],
                  ),
                ),
                SizedBox(height: 10,),
                Card(
                  margin: EdgeInsets.all(12),
                  child: ListTile(
                    leading: Icon(Icons.search,color: Colors.black54,),
                    title: Text("Search",style: TextStyle(color: Colors.black54),
                  ),
                    trailing: Icon(Icons.mic_none_outlined,color: Colors.black54,),
                  ),
                ),
                SizedBox(height:10),
                Card(
                  margin: EdgeInsets.all(12),
                  child:Padding(
                    padding: const EdgeInsets.all(8.0),
                    child: Image(image: AssetImage('assets/images/1.png'),
                    ),
                  ),
                ),
                SizedBox(height: 10,),
                Padding(
                  padding: const EdgeInsets.only(left: 12.0),
                  child: Row(
                    children: [
                      Text("Product name:",
                    style: TextStyle(fontSize: 20,fontWeight: FontWeight.bold,
                    color: Colors.black),
                      ),
                      SizedBox(width: 10,),
                      Text("t-shirt",style: TextStyle(fontSize: 20,fontWeight: FontWeight.normal,)),
                    ],
                  ),
                ),
                SizedBox(height: 10,),
                Card(
                  margin: EdgeInsets.all(12),
                  child:Padding(
                    padding: const EdgeInsets.all(8.0),
                    child: Image(image: AssetImage('assets/images/2.png'),
                    ),
                  ),
                ),
                SizedBox(height: 10,),
                Padding(
                  padding: const EdgeInsets.only(left: 12.0),
                  child: Row(
                    children: [
                      Text("Product name:",
                        style: TextStyle(fontSize: 20,fontWeight: FontWeight.bold,
                            color: Colors.black),
                      ),
                      SizedBox(width: 10,),
                      Text("t-shirt",style: TextStyle(fontSize: 20,fontWeight: FontWeight.normal,)),
                    ],
                  ),
                ),
                SizedBox(height: 10,),
              ],
            ),
          )),
    );
  }
}
