# WordSelectableText 

This is a Text Widget that supports word highlighting and selection. 
It provides an *onWordTapped* function that gives you access to the word selected by the user. 

# HighLight Word

You can highlight the word in any color using the **highlightColor** argument. 


# Language support

The widget uses a regex of alphabet set to select words. For English, regex used is **[a-zA-Z]** 

# Example

    @override
    Widget  build(BuildContext context) {
	    String textToShow =
	    "Dermatology is the branch of medicine dealing with the skin. It is a speciality with both medical and surgical aspects. A dermatologist is a specialist doctor who manages diseases related to skin, hair and nails and some cosmetic problems.";
	    
	    return  Scaffold(
		    appBar:  AppBar(title:  Text("widget testing"),),
		    body:  Container(
			    padding:  EdgeInsets.all(40),
			    width:  double.infinity,
			    child:  WordSelectableText(
				    selectable:  true,
				    highlight:  true,
				    text: textToShow,
				    onWordTapped: (word, index) {},
				    style:  TextStyle(fontSize:  20)
		    )),
	    );
    }


<p>
    <img src="https://github.com/K-Rafiki/wordSelectableText/blob/master/screenshots/example.gif?raw=true"/>
</p>
