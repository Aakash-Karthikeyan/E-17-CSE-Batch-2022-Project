Project Title: Wheat Leaf Disease Recognition using tensorflow and keras

Software required for running the project:
1)Anaconda Navigator
2)Pycharm communtiy Edition

After the installation of Anaconda Navigator, under Home page search for "Environments" section and open it.
Under Environments, search for "create" option and open it. and create a new environment with the name "tensorflow" and click create.

Once done, click on the created environment i.e,tensorflow which will be available under base(root).
once selected,in search packages search for "tensorflow" and select it and click apply.

Click on Windows Start button and open "anaconda prompt".

In anaconda prompt type the following:
activate tensorflow
pip install keras==2.6.0
pip install django==3.2.7

In anaconda navigator,under enviroments select tensorflow and click "update index".

In anaconda navigator,under home, in Application on select"tensorflow". in that install and launch Jupyter note book. inside jupter notebook select the downloaded code folder and open M1.ipynb(Manual Net)and run it.
Same step goes for M2.ipynb (Alexnet algorithm) and M3.ipynb(LeNet algorithm).

Once the algorithm is runned ,it uses the datasets which we have provided it under goes pre-processess and later trains the algorithm and gives out the result as graph which contains training accuracy and loss, testing accuracy and loss. 

And now we shall deploy the best accuracy provided algorithm i.e M3.ipynb(LeNet algorithm) into django to see the how it works.

To deploy djano project follow the steps provided below:
Click on Windows Start button and open "pycharm community edition".
In that open "django Deploy" from the "CODE" Folder.
Once opened under"django Deploy" project, open employee ->views.py
In that following changes has to be made for line 46 and 48.
this changes has to made, copy the address of file location of leaf_.h5 under extracted CODE folder (for example:"C:/Users/ak/Downloads/CODE/django Deploy/employee/leaf_.h5")and paste it line 46.

copy the address of file location of media under extracted "CODE" folder (for example: "C:/Users/Vignesh/Downloads/CODE/django Deploy/media/")and paste it line 48.

once this changes are done click on save.

And now python interpreter has to be added in pycharm. to do that in the bottom rigt corner you will be able to see interpreter settings in that select add interpreter in that click the radio button "existing environment" and give the address which be simliar to mine I have mentioned here("C:\Users\Vignesh\anaconda3\envs\tensorflow\python.exe")

And once this is done it time to run the project.
In pycharm,open new terminal. in the header of the terminal you can see a drop down menu in that select the command prompt option. and type the following

python manage.py runserver


once this command is runned you will be shown an address for the web page. click on that, it will take you the deployed web page.


In the webpage you shall have to upload image you wish to test and click on upload button. which will redirect you the result page where it show whether the leaf is infected or not. if infected it will show treatment recommended and pesticide which can be applied.

----- End of project Execution -----





