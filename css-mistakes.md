Use Shorthand : 



//Not Using Shorthand
.example{
  margin-top:10px;
  margin-bottom:19px;
  margin-left:10px;
  margin-right:19px;
}
//Better way
.example{
  margin:10px 19px;
}

Responsive design : 

//Not correct way
.container{
  width:1000px;
}
//correct way for responsive
.container{
  width:100%;
}

.Repeating the Same Code 

//Not correct
.box1{
  width:50%;
  margin:20px;
}
.box2{
  width:50%;
  margin:20px;
}
//Correct
.box1,.box2{
  width:50%;
  margin:20px;
}

.No font fallback : 

//Not good
body{
  font-family:Helvetica;
}
//Good
body{
  font-family:Helvetica, Arial,Sans-serif;
}

Using Color Names :


//Not good
.example{
  color:green;
}
//Good
.example{
  color:#00ff00;
}

Complicating Selectors :


//It is good some times, but better to don't go eith complicate
header .navigation ul.nav-links{
  list-style-type:none;
}

//Better
.nav-links{
  list-style-type:none;
}

Index mistakes :

.modal-container{
  z-index:545;
}
.modal{
  z-index:5345345;
}


.modal-container{
  z-index:1;
}
.modal{
  z-index:2;
}

Inconsistency names 

<header class='header'></header>
.header{
  font-size:2rem;
}

.When to use class and Id :

<input id="name"  type="text"/>
let name = document.getElementById('name').value;
console.log(name);

<p class="classData">Paragrah</p>
<div class="classData"></div>

.classData{
  margin:20px
}

 Ignoring Cross-Browser Compatibility:
