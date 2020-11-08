# FragmentExample
 
- Example 1
```xml
<fragment
    android:id="@+id/fr_1"
    android:name="com.gzeinnumer.fragmentexample.FirstFragment"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_weight="1" />
```


- Example 2
```xml
<FrameLayout
    android:id="@+id/fr_2"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_weight="1" />
```
```java
FragmentManager fragmentManager = getSupportFragmentManager();
FragmentTransaction fragmentTransaction = fragmentManager.beginTransaction();
Fragment fragment = new FirstFragment();
fragmentTransaction.replace(R.id.fr_2, fragment);
fragmentTransaction.addToBackStack(null);
fragmentTransaction.commit();
```

---

```
Copyright 2020 M. Fadli Zein
```
