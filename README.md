# psandroidfundaintent
## 3. Launching a Specifc Activity with a Eplicit Intent
### 1 Overview
```
startActivityForReault()
```
```
setResult()
onActivityResult()
```

```
Inetnt inetnt = new Intent(this,Ac.class);
startActivity(intent);
```


### 4
```
private void roll(){
  intent.putExtra(DiceActivity.KEY_NUM_DICE,3);
  startActivityForResult(intent,REQUEST_CODE_DICE);
  
}
```


```
protected void onActivityResult(int reauestCode, int resultCode, Intent data){
  if(superCode == REQUEST_CODE_DICE && resultCode == Activity.RESULT_OK){
     super.onActivityResult(resultCode,resultCode,data);
  }
}
```
