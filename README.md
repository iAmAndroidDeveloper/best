<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/all_page_backgroud"
    tools:context=".MainActivity">

    <FrameLayout
        android:id="@+id/tv_dashboard_tag"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="@color/white"
        android:elevation="1dp">


        <TextView
            fontPath="@string/bold"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:gravity="center_vertical"
            android:padding="13dp"
            android:text="dashboard"
            android:textAllCaps="true"
            android:textColor="@color/black"
            android:textSize="22dp"
            tools:ignore="MissingPrefix" />

        <ImageView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="end|center"
            android:padding="10dp"
            android:src="@drawable/ic_setting" />

    </FrameLayout>

    <android.support.v4.widget.NestedScrollView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tv_dashboard_tag">

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:paddingBottom="15dp">

            <RelativeLayout
                android:id="@+id/layout_daily"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginTop="5dp"
                android:background="@color/white"
                android:elevation="1dp"
                android:paddingTop="13dp"
                android:paddingBottom="13dp">

                <ImageView
                    android:id="@+id/img_daily_chart"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:padding="8dp"
                    android:src="@drawable/ic_daily_report" />

                <TextView
                    android:id="@+id/tv_daily_report"
                    fontPath="@string/semibold"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_toEndOf="@+id/img_daily_chart"
                    android:text="daily report"
                    android:textAllCaps="true"
                    android:textColor="@color/home_icons"
                    android:textSize="16dp"
                    tools:ignore="MissingPrefix" />

                <TextView
                    android:id="@+id/tv_daily_report_desc"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_daily_report"
                    android:layout_marginTop="3dp"
                    android:layout_toStartOf="@+id/img_right_daily_report"
                    android:layout_toEndOf="@+id/img_daily_chart"
                    android:text="Check todays report"
                    android:textSize="12dp"
                    tools:ignore="MissingPrefix" />


                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_daily_report_desc"
                    android:layout_marginTop="10dp"
                    android:layout_marginRight="15dp"
                    android:layout_toEndOf="@+id/img_daily_chart"
                    android:orientation="horizontal">

                    <TextView
                        android:id="@+id/btn_cancel"
                        fontPath="@string/semibold"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginRight="10dp"
                        android:layout_weight="1"
                        android:background="@drawable/gradient_view_details_btn"
                        android:gravity="center"
                        android:paddingTop="8dp"
                        android:paddingBottom="8dp"
                        android:text="print K.O.T"
                        android:textAllCaps="true"
                        android:textColor="@color/white"
                        android:textSize="14dp"
                        tools:ignore="MissingPrefix" />

                    <TextView
                        android:id="@+id/btn_create_order"
                        fontPath="@string/semibold"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:background="@drawable/gradient_view_details_btn"
                        android:gravity="center"
                        android:paddingTop="8dp"
                        android:paddingBottom="8dp"
                        android:text="print Report"
                        android:textAllCaps="true"
                        android:textColor="@color/white"
                        android:textSize="14dp"
                        tools:ignore="MissingPrefix" />
                </LinearLayout>

                <ImageView
                    android:id="@+id/img_right_daily_report"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_alignParentEnd="true"
                    android:padding="8dp"
                    android:src="@drawable/ic_right_arrow" />
            </RelativeLayout>

            <RelativeLayout
                android:id="@+id/layout_monthly"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_below="@+id/layout_daily"
                android:layout_marginTop="5dp"
                android:background="@color/white"
                android:elevation="1dp"
                android:paddingTop="13dp"
                android:paddingBottom="13dp">

                <ImageView
                    android:id="@+id/img_monthly_chart"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:padding="8dp"
                    android:src="@drawable/ic_monthly_report" />

                <TextView
                    android:id="@+id/tv_monthly_report"
                    fontPath="@string/semibold"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_toEndOf="@+id/img_monthly_chart"
                    android:text="monthly report"
                    android:textAllCaps="true"
                    android:textColor="@color/home_icons"
                    android:textSize="16dp"
                    tools:ignore="MissingPrefix" />

                <TextView
                    android:id="@+id/monthly_tag"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_monthly_report"
                    android:layout_marginTop="3dp"
                    android:layout_toStartOf="@+id/img_right_monthly_report"
                    android:layout_toEndOf="@+id/img_monthly_chart"
                    android:text="Check monthly report"
                    android:textSize="12dp"
                    tools:ignore="MissingPrefix" />


                <TextView
                    fontPath="@string/semibold"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/monthly_tag"
                    android:layout_marginTop="5dp"
                    android:layout_marginBottom="2dp"
                    android:layout_toStartOf="@+id/img_right_monthly_report"
                    android:layout_toEndOf="@+id/img_monthly_chart"
                    android:text="01 to 31 OCT 2018 ORDERS"
                    android:textColor="@color/black"
                    android:textSize="14dp"
                    tools:ignore="MissingPrefix" />


                <ImageView
                    android:id="@+id/img_right_monthly_report"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_alignParentEnd="true"
                    android:padding="8dp"
                    android:src="@drawable/ic_right_arrow" />
            </RelativeLayout>

            <!--category-->
            <RelativeLayout
                android:id="@+id/container_for_category"
                android:layout_width="match_parent"
                android:layout_height="120dp"
                android:layout_below="@+id/layout_monthly"
                android:layout_marginTop="10dp"
                android:background="@color/white"
                android:elevation="1dp">

                <View
                    android:id="@+id/view_category"
                    android:layout_width="10dp"
                    android:layout_height="match_parent"
                    android:background="#4285F4" />

                <TextView
                    android:id="@+id/tv_category_tag"
                    fontPath="@string/semibold"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_toEndOf="@+id/view_category"
                    android:paddingLeft="10dp"
                    android:paddingTop="5dp"
                    android:text="categorys"
                    android:textAllCaps="true"
                    android:textColor="@color/home_icons"
                    android:textSize="20dp"
                    tools:ignore="MissingPrefix" />

                <TextView
                    android:id="@+id/category_extra_Tag"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_category_tag"
                    android:layout_marginLeft="10dp"
                    android:layout_toEndOf="@+id/view_category"
                    android:text="List of all category with related products"
                    android:textSize="12dp"
                    tools:ignore="MissingPrefix" />


                <ImageView
                    android:id="@+id/img_right_category"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_alignParentEnd="true"
                    android:padding="8dp"
                    android:src="@drawable/ic_right_arrow" />


                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_alignParentBottom="true"
                    android:layout_marginLeft="10dp"
                    android:layout_marginRight="10dp"
                    android:layout_marginBottom="10dp"
                    android:layout_toEndOf="@+id/view_category"
                    android:orientation="horizontal">

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_cat_total"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:text="Total"
                            android:textSize="14dp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_cat_active"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="center"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="center"
                            android:text="Active"
                            android:textSize="14dp" />
                    </LinearLayout>


                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_cat_deactive"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="right"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="right"
                            android:text="Deactive"
                            android:textSize="14dp" />
                    </LinearLayout>


                </LinearLayout>
            </RelativeLayout>

            <!--Products-->
            <RelativeLayout
                android:id="@+id/container_for_products"
                android:layout_width="match_parent"
                android:layout_height="120dp"
                android:layout_below="@+id/container_for_category"
                android:layout_marginTop="10dp"
                android:background="@color/white"
                android:elevation="1dp">

                <View
                    android:id="@+id/view_product"
                    android:layout_width="10dp"
                    android:layout_height="match_parent"
                    android:background="#189279" />

                <TextView
                    android:id="@+id/tv_product_tag"
                    fontPath="@string/semibold"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_toEndOf="@+id/view_product"
                    android:paddingLeft="10dp"
                    android:paddingTop="5dp"
                    android:text="Products"
                    android:textAllCaps="true"
                    android:textColor="@color/home_icons"
                    android:textSize="20dp"
                    tools:ignore="MissingPrefix" />

                <TextView
                    android:id="@+id/product_extra_Tag"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_product_tag"
                    android:layout_marginLeft="10dp"
                    android:layout_toEndOf="@+id/view_product"
                    android:text="List of all products for serve customer"
                    android:textSize="12dp"
                    tools:ignore="MissingPrefix" />


                <ImageView
                    android:id="@+id/img_right_products"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_alignParentEnd="true"
                    android:padding="8dp"
                    android:src="@drawable/ic_right_arrow" />


                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_alignParentBottom="true"
                    android:layout_marginLeft="10dp"
                    android:layout_marginRight="10dp"
                    android:layout_marginBottom="10dp"
                    android:layout_toEndOf="@+id/view_product"
                    android:orientation="horizontal">

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_total_products"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:text="Total"
                            android:textSize="14dp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_active_product"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="center"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="center"
                            android:text="Active"
                            android:textSize="14dp" />
                    </LinearLayout>


                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_weight="1"
                        android:orientation="vertical">

                        <TextView
                            android:id="@+id/tv_deactive_product"
                            fontPath="@string/bold"
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="right"
                            android:textColor="@color/black"
                            android:textSize="25dp"
                            tools:ignore="MissingPrefix" />

                        <TextView
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:gravity="right"
                            android:text="Deactive"
                            android:textSize="14dp" />
                    </LinearLayout>


                </LinearLayout>
            </RelativeLayout>

            <RelativeLayout
                android:id="@+id/container_for_table"
                android:layout_width="match_parent"
                android:layout_height="120dp"
                android:layout_below="@+id/container_for_products"
                android:layout_marginTop="10dp"
                android:background="@color/white"
                android:elevation="1dp">

                <View
                    android:id="@+id/view_table"
                    android:layout_width="10dp"
                    android:layout_height="match_parent"
                    android:background="#FF5A60" />

                <TextView
                    android:id="@+id/tv_table_tag"
                    fontPath="@string/semibold"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_toEndOf="@+id/view_table"
                    android:paddingLeft="10dp"
                    android:paddingTop="5dp"
                    android:text="tables"
                    android:textAllCaps="true"
                    android:textColor="@color/home_icons"
                    android:textSize="20dp"
                    tools:ignore="MissingPrefix" />

                <TextView
                    android:id="@+id/table_extra_Tag"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_below="@+id/tv_table_tag"
                    android:layout_marginLeft="10dp"
                    android:layout_toEndOf="@+id/view_table"
                    android:text="List of all table for customer"
                    android:textSize="12dp"
                    tools:ignore="MissingPrefix" />


                <ImageView
                    android:id="@+id/img_right_table"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_alignParentEnd="true"
                    android:padding="8dp"
                    android:src="@drawable/ic_right_arrow" />


                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_alignParentBottom="true"
                    android:layout_marginLeft="10dp"
                    android:layout_marginRight="10dp"
                    android:layout_marginBottom="10dp"
                    android:layout_toEndOf="@+id/view_table"
                    android:orientation="vertical">

                    <TextView
                        android:id="@+id/tv_table_total"
                        fontPath="@string/bold"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:textColor="@color/black"
                        android:textSize="25dp"
                        tools:ignore="MissingPrefix" />

                    <TextView
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:text="Total"
                        android:textSize="14dp" />
                </LinearLayout>
            </RelativeLayout>
        </RelativeLayout>
    </android.support.v4.widget.NestedScrollView>
</RelativeLayout>
