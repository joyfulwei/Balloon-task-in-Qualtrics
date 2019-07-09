# Balloon-task-in-Qualtrics
Here are the codes that you can refer to deploy Balloon Analogue Risk Task into Qualtrics.

The steps suggested to follow:
 1. Put the HTML codes into Qualtrics. You can do this clicking the "HTML View" where you edit questions in Qualtrics.
 2. Put Javascript codes in Qualtrics. You can refer to the Qualtrics Support to know how to add javascript, here is the link:       https://www.qualtrics.com/support/survey-platform/survey-module/question-options/add-javascript/
 3.Download the balloon picture and upload the Balloon image to your Qualtrics library, and change the link address of the picture. After you upload the image successfully, you could find the concerned link in your Qualtrics library.
 here is the code you need to revise:   <img src=https://erasmusuniversity.eu.qualtrics.com/ControlPanel/Graphic.php?IM=IM_e40vZ7nffgjMnul id="ballon" alt="Ballon">, you can find this in the HTML codes. 
 4.In the "survey flow", add "Set Embedded Data" to save the related data. The codes are as below: 
       exploded = ${e://Field/number_pumps}
       number_pumps= ${e://Field/number_pumps}
 5.Run the game and check the data.

Notice: please be aware of that this task in not completeley the same as the seminal work, which was published by Lejuez and Read et al. in 2002, because when the balloon will burst in this task is set randomly, but in the seminal paper, the time when balloon is exploded is probabilistic. So this version is not perfect yet. If you are intertesd, you can work on this version to make a probabilistic one.
