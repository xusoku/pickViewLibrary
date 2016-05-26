# pickViewLibrary



![image](https://github.com/xusoku/pickViewLibrary/blob/master/62B5B215537BB702D9EAF8059F9BA17B.jpg)



------
```java
// 时间选择器
		TimePickerView pvTime = new TimePickerView(this, TimePickerView.Type.YEAR_MONTH_DAY);
		// 控制时间范围
//		 Calendar calendar = Calendar.getInstance();
//		 pvTime.setRange(calendar.get(Calendar.YEAR) - 20,
//		 calendar.get(Calendar.YEAR));
		pvTime.setTime(new Date());
		pvTime.setCyclic(false);
		pvTime.setCancelable(true);
		pvTime.show();
		// 时间选择后回调
		pvTime.setOnTimeSelectListener(new TimePickerView.OnTimeSelectListener() {

			@Override
			public void onTimeSelect(Date date) {
				XXX.setText(getTime(date));
			}
		});
	
	
	
	
	final ArrayList<String> list=new ArrayList<String>();
		list.add("11");
		list.add("22");
		list.add("33");
		list.add("44");


		final ArrayList<ArrayList<String>> arrayLists=new ArrayList<ArrayList<String>>();
		ArrayList<String> a=new ArrayList<String>();
		a.add("111");
		a.add("112");
		a.add("113");
		a.add("114");
		arrayLists.add(a);
		ArrayList<String> b=new ArrayList<String>();
		b.add("221");
		b.add("222");
		b.add("223");
		b.add("224");
		arrayLists.add(b);
		ArrayList<String> c=new ArrayList<String>();
		c.add("331");
		c.add("332");
		c.add("333");
		c.add("334");
		arrayLists.add(c);
		ArrayList<String> d=new ArrayList<String>();
		d.add("441");
//		d.add("442");
		d.add("443");
		d.add("444");
		arrayLists.add(d);

		tpvOptions.setPicker(list, arrayLists, false);
		tpvOptions.setCyclic(false);
		tpvOptions.setSelectOptions(0, 0);
		tpvOptions.show()
		tpvOptions.setOnoptionsSelectListener(new TwoPickerView.OnOptionsSelectListener() {
			@Override
			public void onOptionsSelect(int options1, int option2) {

				XXX.setText(list.get(options1)+"  "+arrayLists.get(options1).get(option2));
			}
		});
			

```

-------
