# Decision-making-tool

## This is a simple guide to data-file extension.

There are two types of elements with which the user can enter his choice/information

1 - SELECTIVE ITEM : user make choise by clicking item. 

 ======================== IN CODE =====================
 
 {
  
  id: 0,  // example id.
  
  type: "select_item",
  
  content: "Which are basic living conditions?", // item block text 
  
}
 
 ======================================================

2 - FREE ANSWER ITEM : user have to fill text form and apply data.

 ======================== IN CODE =====================
 
{

  id: 5,  // example id.
  
  type: "free_answer_item",
  
  content: "Free answer", // item block text 
  
  url : -some url-  // Optional. You can add image/icon url and it will be displayed 
},
 
 ======================================================

## Examples

## SELECTIVE ITEM

![select_item](https://user-images.githubusercontent.com/78759306/188727919-afd85c99-eeb7-4e10-8fea-783b38bf0a01.jpg)

## SELECTIVE ITEM with icon

<img width="441" alt="image" src="https://user-images.githubusercontent.com/78759306/188738604-f67ed792-d5c4-43b4-8551-a02194b8aa0b.png">

##  FREE ANSWER ITEM

![free_answer](https://user-images.githubusercontent.com/78759306/188729886-c0021ba4-7f1a-4248-b4ae-9e89a09bb4d0.jpg)

## FREE ANSWER ITEM Customization

When we expect an open response from the user, we can give him some hints in the form of an explanation of the question or additional questions.

### FREE ANSWER WITH ADDITIONAL QUESTIONS

 ======================== IN CODE =====================
 
{

  id: 5, // example id.
  
  type: "free_answer_item",
  
  content: "Free answer",
  
  questions: ["Possible question 1", ...other questions...], // Optional.You can extend array with question
  
},
 
 ======================================================
 
 ## EXAMPLE

<img width="459" alt="image" src="https://user-images.githubusercontent.com/78759306/188731698-15d2a2c5-b8df-44dc-af24-5353d545bd17.png">

### FREE ANSWER WITH ADDITIONAL QUESTIONS AND EXPLANATORY

 ======================== IN CODE =====================
 
{

  id: 5,  // example id.
  
  type: "free_answer_item", // 
  
  content: "Free answer",
  
  explanatory: "EXPLANATORY TEXT...", // Optional. You can set your own explanatory text.
  
  questions: ["Possible question 1", ...other questions...],  // Optional. You can extend array with question
  
},
 
 ======================================================
 
 ## EXAMPLE

<img width="462" alt="image" src="https://user-images.githubusercontent.com/78759306/188731937-9efbb5ae-dbb0-42b4-9754-2007ddc12ed3.png">


# CONFIRMATION ITEMS

 ======================== IN CODE =====================
 
{

    type: "confirm",
    
    title: "Further explore?", // you can change it
    
    navbar: false, 

    values: [ //  You can add or remove items
    
      {
      
        text: "YES", // item text. You can change it
        
        next: 6, //  next item id. You can change it
        
      },
      
      {
      
        text: "NO", // item text. You can change it
        
        next: 10, //  next item id. You can change it
        
      },
      
    ],
    
  },
  
 
 ======================================================
 
 This items used for navigating between sections. For example if user does not need "criterias explore" he/she can skip this step and move to next section. 
 
 ## EXAPMLE
 <img width="617" alt="image" src="https://user-images.githubusercontent.com/78759306/188737513-bac823b5-27bd-490a-92c2-d963ed8d1b15.png">





