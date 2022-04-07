
# Rapport

**Skriv din rapport här!**

This assignment was about using WebView, so i started by renaming the existing TextView to WebView.
I then called upon this WebView (via an id i gave it), in MainActivity.java. There, I also enabled JavaScript.
After that I made a simple html site consisting of just a header and a GIF image.
Then I placed that site in the assets folder and then called upon it in the existing showInternalWebPage() function. Then i added HIS.se in the existing showExternalWebPage() function.
Then all that was left was to call upon these functions when the dropdown was clicked.

The first paragraph of program code shows how i implemented the internal webpage in the showInternalWebPage() function.
The second paragraph shows how said function (and showExternalWebPage, the one for the external web page) are called when the dropdown is used.

## Följande grundsyn gäller dugga-svar:

- Ett kortfattat svar är att föredra. Svar som är längre än en sida text (skärmdumpar och programkod exkluderat) är onödigt långt.
- Svaret skall ha minst en snutt programkod.
- Svaret skall inkludera en kort övergripande förklarande text som redogör för vad respektive snutt programkod gör eller som svarar på annan teorifråga.
- Svaret skall ha minst en skärmdump. Skärmdumpar skall illustrera exekvering av relevant programkod. Eventuell text i skärmdumpar måste vara läsbar.
- I de fall detta efterfrågas, dela upp delar av ditt svar i för- och nackdelar. Dina för- respektive nackdelar skall vara i form av punktlistor med kortare stycken (3-4 meningar).

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

```
public void showInternalWebPage(){
    myWebView.loadUrl("file:///android_asset/for_assets.html");
}
```

```
public boolean onOptionsItemSelected(MenuItem item) {
    // Handle action bar item clicks here. The action bar will
    // automatically handle clicks on the Home/Up button, so long
    // as you specify a parent activity in AndroidManifest.xml.
    int id = item.getItemId();

    //noinspection SimplifiableIfStatement
    if (id == R.id.action_external_web) {
        Log.d("==>","Will display external web page");
        showExternalWebPage();
        return true;
    }

    if (id == R.id.action_internal_web) {
        Log.d("==>","Will display internal web page");
        showInternalWebPage();
        return true;
    }

    return super.onOptionsItemSelected(item);
}
```

Bilder läggs i samma mapp som markdown-filen.

![](external.png)
![](internal.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
