## 效果
<img src="img/img.gif#pic_center" alt="SwitchButton" width="60%" align="center" />

## 使用方法
###### 1.style.xml中引入自定义标签
```java
 <declare-styleable name="SwitchButton">
 <attr name="sb_shadow_radius" format="reference|dimension" />
 <attr name="sb_shadow_offset" format="reference|dimension" />
 <attr name="sb_shadow_color" format="reference|color" />
 <attr name="sb_uncheck_color" format="reference|color" />
 <attr name="sb_checked_color" format="reference|color" />
 <attr name="sb_border_width" format="reference|dimension" />
 <attr name="sb_checkline_color" format="reference|color" />
 <attr name="sb_checkline_width" format="reference|dimension" />
 <attr name="sb_uncheckcircle_color" format="reference|color" />
 <attr name="sb_uncheckcircle_width" format="reference|dimension" />
 <attr name="sb_uncheckcircle_radius" format="reference|dimension" />
 <attr name="sb_checked" format="reference|boolean" />
 <attr name="sb_shadow_effect" format="reference|boolean" />
 <attr name="sb_effect_duration" format="reference|integer" />
 <attr name="sb_button_color" format="reference|color" />
 <attr name="sb_show_indicator" format="reference|boolean" />
 <attr name="sb_background" format="reference|color" />
 <attr name="sb_enable_effect" format="reference|boolean" />
 </declare-styleable>
```

###### 2.引入自定义View布局
```java
<per.stramchen.switchbuttondemo.SwitchButton
	android:id="@+id/btn_voice_switch"
	android:layout_width="wrap_content"
	android:layout_height="wrap_content"
	android:layout_weight="1"
	app:sb_background="#E8E9EB"
	app:sb_checked_color="#65C065"
	app:sb_show_indicator="false" />
```


###### 3.设置监听

```java
        switchButton.setOnCheckedChangeListener(
        new SwitchButton.OnCheckedChangeListener() {
            @Override
            public void onCheckedChanged(SwitchButton view, final boolean isChecked) {

            }
        });
```