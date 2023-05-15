# Form_OnChange_onClick


import React,{useState} from 'react';

function App() {
  const[data,setData]=useState("Ankur's Medhavi");
  function handleChange(event){
    setData(event.target.value)
    }
  return (
    <>
    <div className='container'>
      <h2>Form Validation</h2>
     <input type = "text" placeholder='Name'></input>
     <input type = "number" placeholder='Age'></input>
     <select placeholder='Choose your gender'>
      <option>Male</option>
      <option>Female</option>
      <option>Others</option>
     </select>
     <input type = "text" placeholder='Phone number'></input>
     <button value = {data} onClick={handleChange}>Click here</button>
     </div>
    </>
   
  );
}

export default App;
