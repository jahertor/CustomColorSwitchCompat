# Change SwitchCompat color programmatically [CustomColorSwitchCompat]
Change color of SwitchCompat programmatically or in xml layout

## Programmatically
```
final CustomColorSwitchCompat switchRequestPin = (CustomColorSwitchCompat) findViewById(R.id.switchRequestPin);
switchRequestPin.setBgOnColor(Color.parseColor("#009284"));
switchRequestPin.setBgOffColor(Color.parseColor("#d0d0d0"));
switchRequestPin.setToggleOnColor(Color.parseColor("#97d9d7"));
switchRequestPin.setToggleOffColor(Color.parseColor("#a6a6a6"));
switchRequestPin.setOnCheckedChangeListener(new CompoundButton.OnCheckedChangeListener() {
    @Override
    public void onCheckedChanged(CompoundButton buttonView, boolean isChecked) {
        // TODO do something
    }
});
```

## XML Layout
```
<com.jahertor.customcolorswitchcompat.CustomColorSwitchCompat
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:id="@+id/switchRequestPin"
    android:layout_centerVertical="true"
    android:layout_alignParentRight="true"
    android:layout_alignParentEnd="true"
    android:layout_toRightOf="@id/hello"
    app:toggleOnColor="#009284"
    app:toggleOffColor="#d0d0d0"
    app:bgOnColor="#97d9d7"
    app:bgOffColor="#a6a6a6" />
```

## Getting started
Just import the code as a module in Android Studio.

## License
```
Copyright 2015 Javier Hernández Torres

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
