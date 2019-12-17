
const MongoClient = require('mongodb').MongoClient;
const uri = "mongodb+srv://dbuser:nikhil@cluster0-dqu8h.mongodb.net/test?retryWrites=true&w=majority";
const client = new MongoClient(uri,{ useUnifiedTopology: true } , { useNewUrlParser: true });
client.connect(err => {
  if (err) throw err;
  const collection = client.db("Garda_Electronics").collection("Mobile_Accessories");

  var before = {price:'$12'};
  var after = {$set: {price:'$20'}};
	 collection.updateOne(before,after,function(err,res){
		 if (err) throw err;
		 console.log("row updated");
   });
   
   if (err) throw err;
  const collection_0 = client.db("Garda_Electronics").collection("Mobile_Insurance");

  var before_0 = {insurencenumber:'4555'};
  var after_0 = {$set: {insurencenumber:'44444'}};
	 collection_0.updateOne(before_0,after_0,function(err,res){
		 if (err) throw err;
		 console.log("row updated");
   });
   
   if (err) throw err;
   const collection_1 = client.db("Garda_Electronics").collection("Repair");
 
   var before_1 = {repair_id:'01'};
   var after_1 = {$set: {repair_id:'11'}};
    collection_1.updateOne(before_1,after_1,function(err,res){
      if (err) throw err;
      console.log("row updated");
    });
    if (err) throw err;
    const collection_1 = client.db("Garda_Electronics").collection("Employees");
  
    var before_1 = {Employee_name: 'Rohan'};
    var after_1 = {$set: {Employee_name: 'Shamil'}};
     collection_1.updateOne(before_1,after_1,function(err,res){
       if (err) throw err;
       console.log("row updated");
     });
  console.log("connected");
  client.close();
});
