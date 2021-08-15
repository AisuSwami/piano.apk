# piano.apk
/*Everyone learning new hobbies music is one of them, but not everyone has prior knowledge where to start and how to start, for music instruments, we need to spend a lot of money. It is not possible to purchase Casio (piano ) for every music lover who want to learn or practice  tunes or songs, but today everyone has mobile-phones, smart phones, androids. So ,its better to practice in  virtual piano, the Android application can have online features or recording the songs or nodes they are playing, user can only play the nodes on board ,Tutorials, where  user can learn nodes and fingers and thumb positions. User can record the song or nodes he/she is playing. They can play recorded songs, Competition can be conduct between users. Recorded video can be upload or share  on other apps   We are introducing the “Piano.apk”, the android app or application. So, they can play, learn and practice music rhythms everywhere and  anytime according to their wish. Same music nodes and tunes provide real experience of playing piano. This is developed using Java in Android Studio. Where user can play, learn and practice their tunes, songs. Here we use Media for transporting node sounds in keys of piano so it gives real feel, we can register then login.*/


//Activity.XML code:

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/colorPrimaryDark"
    tools:context=".MainActivity">

    <RelativeLayout
        android:id="@+id/top_layout"
        android:layout_width="match_parent"
        android:layout_height="100dp"
        android:background="@color/colorPrimaryDark">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="horizontal">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:orientation="vertical"
                android:layout_weight="0.5">

                <LinearLayout
                    android:layout_marginTop="10dp"
                    android:layout_gravity="center"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:orientation="horizontal">

                    <ImageButton
                        android:id="@+id/Btnrecord"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:src="@drawable/record_ic_background"/>

                    <ImageButton
                        android:id="@+id/BtnStop"
                        android:layout_width="79dp"
                        android:layout_height="wrap_content"
                        android:src="@drawable/stop_ic_background" />
                    <ImageButton
                        android:id="@+id/BtnPlay"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:src="@drawable/play_ic_background"/>

                </LinearLayout>



            </LinearLayout>


            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:orientation="vertical"
                android:gravity="center"
                android:layout_weight="0.5">

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="My Piano"
                    android:textStyle="bold"
                    android:textColor="#D3C5C5"
                    android:layout_gravity="center"
                    android:textAppearance="@style/TextAppearance.AppCompat.Display1"/>


            </LinearLayout>


            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:orientation="vertical"
                android:layout_weight="0.5">

                <LinearLayout
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_gravity="center"
                    android:layout_marginTop="10dp"
                    android:orientation="horizontal">
                    <Switch
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:id="@+id/adsSwitch"
                        android:layout_gravity="center"
                        android:checked="true"/>
                    <ImageButton
                        android:id="@+id/BtnSetting"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:src="@drawable/setting_ic_background"/>
                    <ImageButton
                        android:id="@+id/BtnAppExit"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:src="@drawable/exit_ic_background"/>
                </LinearLayout>



            </LinearLayout>

        </LinearLayout>

    </RelativeLayout>

    <RelativeLayout
        android:layout_below="@+id/top_layout"
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="horizontal">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="0.5"
                android:orientation="horizontal">
                <View
                    android:id="@+id/d1"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d2"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d3"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d4"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
            </LinearLayout>
            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="0.5"
                android:orientation="horizontal">
                <View
                    android:id="@+id/d5"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d6"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d7"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d8"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
            </LinearLayout>
            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_weight="0.5"
                android:orientation="horizontal">
                <View
                    android:id="@+id/d9"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d10"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d11"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
                <View
                    android:id="@+id/d12"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_marginLeft="4dp"
                    android:layout_weight="0.5"
                    android:background="@android:color/white"/>
            </LinearLayout>

        </LinearLayout>
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="150dp"
            android:orientation="horizontal">

            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_marginLeft="20dp"
                android:layout_marginRight="20dp"
                android:layout_weight="0.5">
                <View
                    android:id="@+id/t1"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t2"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t3"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
            </LinearLayout>
            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_marginLeft="20dp"
                android:layout_marginRight="20dp"
                android:layout_weight="0.5">
                <View
                    android:id="@+id/t4"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t5"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t6"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
            </LinearLayout>
            <LinearLayout
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_marginLeft="20dp"
                android:layout_marginRight="20dp"
                android:layout_weight="0.5">
                <View
                    android:id="@+id/t7"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t8"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
                <View
                    android:id="@+id/t9"
                    android:layout_width="wrap_content"
                    android:layout_height="match_parent"
                    android:layout_weight="0.5"
                    android:layout_marginLeft="4dp"
                    android:background="@color/colorPrimaryDark"/>
            </LinearLayout>

        </LinearLayout>


    </RelativeLayout>


//Main Activity code:

package com.example.mypiano;

import android.annotation.SuppressLint;
import android.media.MediaPlayer;
import android.os.CountDownTimer;
import android.app.Activity;
import android.os.Bundle;
import android.view.MotionEvent;
import android.view.View;
import android.widget.ImageButton;
import android.widget.Switch;
import android.widget.Toast;

public class MainActivity extends Activity {


    View d1, d2, d3, d4, d5, d6, d7,d8, d9,d10, d11, d12;
    View t1, t2, t3, t4, t5, t6, t7, t8, t9;
    Switch AdsSwitch;
    ImageButton record, stop, play;
    ImageButton Appsetting, appExit;

    private MediaPlayer mD1, mD2, mD3,mD4,mD5,mD6,mD7,mD8,mD9,mD10,mD11,mD12;
    private MediaPlayer mT1, mT2,mT3,mT4,mT5,mT6,mT7,mT8,mT9;




    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);



        mD1 = MediaPlayer.create(this, R.raw.d1);
        mD2 = MediaPlayer.create(this, R.raw.d2);
        mD3 = MediaPlayer.create(this, R.raw.d3);
        mD4 = MediaPlayer.create(this, R.raw.d4);
        mD5 = MediaPlayer.create(this, R.raw.d5);
        mD6 = MediaPlayer.create(this, R.raw.d6);
        mD7 = MediaPlayer.create(this, R.raw.d7);
        mD8 = MediaPlayer.create(this, R.raw.d8);
        mD9 = MediaPlayer.create(this, R.raw.d9);
        mD10 = MediaPlayer.create(this, R.raw.d10);
        mD11 = MediaPlayer.create(this, R.raw.d11);
        mD12 = MediaPlayer.create(this, R.raw.d12);

        mT1 = MediaPlayer.create(this, R.raw.t1);
        mT2 = MediaPlayer.create(this, R.raw.t2);
        mT3 = MediaPlayer.create(this, R.raw.t3);
        mT4 = MediaPlayer.create(this, R.raw.t4);
        mT5 = MediaPlayer.create(this, R.raw.t5);
        mT6 = MediaPlayer.create(this, R.raw.t6);
        mT7 = MediaPlayer.create(this, R.raw.t7);
        mT8 = MediaPlayer.create(this, R.raw.t8);
        mT9 = MediaPlayer.create(this, R.raw.t9);

        d1 = findViewById(R.id.d1);
        d2 = findViewById(R.id.d2);
        d3 = findViewById(R.id.d3);
        d4 = findViewById(R.id.d4);
        d5 = findViewById(R.id.d5);
        d6 = findViewById(R.id.d6);
        d7 = findViewById(R.id.d7);
        d8 = findViewById(R.id.d8);
        d9 = findViewById(R.id.d9);
        d10 = findViewById(R.id.d10);
        d11 = findViewById(R.id.d11);
        d12 = findViewById(R.id.d12);

        t1 = findViewById(R.id.t1);
        t2 = findViewById(R.id.t2);
        t3 = findViewById(R.id.t3);
        t4 = findViewById(R.id.t4);
        t5 = findViewById(R.id.t5);
        t6 = findViewById(R.id.t6);
        t7 = findViewById(R.id.t7);
        t8 = findViewById(R.id.t8);
        t9 = findViewById(R.id.t9);

        AdsSwitch = findViewById(R.id.adsSwitch);
        record = findViewById(R.id.Btnrecord);
        stop = findViewById(R.id.BtnStop);
        play = findViewById(R.id.BtnPlay);
        Appsetting = findViewById(R.id.BtnSetting);
        appExit = findViewById(R.id.BtnAppExit);

        appExit.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                finish();
            }
        });
        Appsetting.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(MainActivity.this, "Piano Setting", Toast.LENGTH_SHORT).show();
            }
        });


        d1.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD1.start();
                d1.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d1.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });

        d2.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD2.start();
                d2.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d2.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d3.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD3.start();
                d3.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d3.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d4.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD4.start();
                d4.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d4.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d5.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD5.start();
                d5.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d5.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d6.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD6.start();
                d6.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d6.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d7.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD7.start();
                d7.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d7.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d8.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD8.start();
                d8.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d8.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d9.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD9.start();
                d9.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d9.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d10.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD10.start();
                d10.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d10.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d11.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD11.start();
                d11.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d11.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });
        d12.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {

                mD12.start();
                d12.setBackgroundColor(getColor(R.color.touched));
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d12.setBackgroundColor(getColor(R.color.return_key));
                    }
                }.start();

                return false;
            }
        });

        t1.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT1.start();
                t1.setBackgroundColor(getColor(R.color.t_toched));

                d1.setEnabled(false);
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d1.setEnabled(true);
                        t1.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t2.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT2.start();
                t2.setBackgroundColor(getColor(R.color.t_toched));
                d2.setEnabled(false);
                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d2.setEnabled(true);
                        t2.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t3.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT3.start();
                t3.setBackgroundColor(getColor(R.color.t_toched));
                d3.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d3.setEnabled(true);
                        t3.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t4.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT4.start();
                t4.setBackgroundColor(getColor(R.color.t_toched));
                d4.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d4.setEnabled(true);
                        t4.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t5.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT5.start();
                t5.setBackgroundColor(getColor(R.color.t_toched));
                d5.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d5.setEnabled(true);
                        t5.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t6.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT6.start();
                t6.setBackgroundColor(getColor(R.color.t_toched));
                d6.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d6.setEnabled(true);
                        t6.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t7.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT7.start();
                t7.setBackgroundColor(getColor(R.color.t_toched));
                d7.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d7.setEnabled(true);
                        t7.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t8.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT8.start();
                t8.setBackgroundColor(getColor(R.color.t_toched));
                d8.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d8.setEnabled(false);
                        t8.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });
        t9.setOnTouchListener(new View.OnTouchListener() {
            @SuppressLint("NewApi")
            @Override
            public boolean onTouch(View v, MotionEvent event) {
                mT9.start();
                t9.setBackgroundColor(getColor(R.color.t_toched));
                d9.setEnabled(false);

                new CountDownTimer(1*100, 100){

                    @Override
                    public void onTick(long millisUntilFinished) {
                        String.valueOf(millisUntilFinished/100);
                    }

                    @SuppressLint("NewApi")
                    @Override
                    public void onFinish() {
                        d9.setEnabled(true);
                        t9.setBackgroundColor(getColor(R.color.colorPrimaryDark));
                    }
                }.start();

                return false;
            }
        });


    }




}
