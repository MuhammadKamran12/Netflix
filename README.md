index.js file
import React from "react";
import ReactDom from "react-dom";
import Card from "./Cards";
ReactDom.render(
<>
<Card imgsrc= " ./public/1.jpg"
title = "A Netflix Series"
sername = "DARK QUEEN"

/>
<Card
 imgsrc= "./public/2.pug"
title = "A Netflix Series"
sername = "DARK QUEEN"
/>
<Card
 imgsrc= " https://wallpapercave.com/wp/wp4056410.jpg"
title = "A Netflix Series"
sername = "DARK QUEEN"
/>

</>,
document.getElementById('root')
);

card.jsx file
import React from 'react';
import "./index.css";
function Card(props)
{
  console.log(props);
  return
  (
<>
<div className= "Cards">
  <div className = "Card">
    <img src = {props.imgsrc} alt= "MyPic" className="Card_info"/>
    <div className = "Card_Info">
    <span className = "class_catogary"> {props.title} </span>
    <h3 className= "Card_title">{props.sername}</h3>
    <a>
    <button>WATCH NOW</button>
  </a>
</div>
</div>
</div>
</>
  );
}
export default Card;
