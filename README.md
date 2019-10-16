# Balloon-task-in-Qualtrics
Here are the codes and images that you may need to deploy Balloon Analogue Risk Task into Qualtrics. 
1. HTML page
2. Javascript code
3. Balloon.png

The steps you should follow to make the BART function well in Qualtrics:
 
 1. Put the HTML codes into Qualtrics. You can start a new queestion in your survey, then click the "HTML View" where you edit questions in Qualtrics. Just copy and paste the codes I have uploaded (HTML page).
 
 2. Put Javascript codes in Qualtrics. You can refer to the Qualtrics Support to know how to add javascript, here is the link: https://www.qualtrics.com/support/survey-platform/survey-module/question-options/add-javascript/. Just copy and paste all the codes I have created (Javascript code).
 
 3.Download the balloon picture and upload the Balloon.png to your Qualtrics library, and change the related link address of the picture. After you upload the image successfully, you could find the concerned link address in your Qualtrics library.
 And find the code you need to revise:   <img src=https://erasmusuniversity.eu.qualtrics.com/ControlPanel/Graphic.php?IM=IM_e40vZ7nffgjMnul id="ballon" alt="Ballon">, which you could find this in the HTML.
 
 4.In the "survey flow", add "Set Embedded Data" to save the related data. The codes are as below: 
       exploded = ${e://Field/number_pumps}
       number_pumps= ${e://Field/number_pumps}
       
 5.Run the game and check the data.

Notice: please be aware of that this task in not completeley the same as the seminal work, which was published by Lejuez and Read et al. in 2002, because when the balloon will burst in this task is set randomly, but in the seminal paper, the time when balloon is exploded is probabilistic. So this version is not perfect yet. If you are intertesd, you can work on this version to make a probabilistic one.

Now the newest version of the BART which could be implemented in Qualtrics has a probablistic manner, thanks to Georg D. Granic's contribuion. 
