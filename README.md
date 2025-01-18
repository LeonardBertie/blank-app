import streamlit as st
st.sidebar.title("欢迎光临")
dataset=st.sidebar.selectbox('选择你想显示的应用',('请选择','雪花','气球','Emoji猜成语'))
if dataset=='请选择':
    st.header("Welcome to Cindy's New App👋")
    st.image("https://s2.loli.net/2025/01/18/wngh7L4Qi35foUe.jpg")
    st.image("https://s2.loli.net/2025/01/18/OGjIdbLwriJyqxE.jpg")
if dataset=='雪花':
    st.header('雪花飘落❄❄')
    st.image("https://s2.loli.net/2025/01/18/yXSA2b9iUldsfEN.jpg")
    st.snow()
    st.write("想要再看一次雪花吗？🥰")
    button_1=st.button('再来一次')
if dataset=='气球':
    st.header('气球🎈')
    st.image("https://s2.loli.net/2025/01/18/NzeJyICi5sT1tUl.jpg")
    st.balloons()
    st.write("想要再看一次气球吗？🥰")
    button_1=st.button('再来一次')
if dataset=='Emoji猜成语':
    st.header('Emoji猜成语')
    st.write("1.👆🚀🀄💑")
    x1=st.text_input("请输入第一题的答案")
    m=0
    if x1=="一见钟情":
        st.write("Yes!!!😊")
        m=1
    else:
        st.write("No😭")
    if m==1:
        st.write('2.✖💨💔🌊')
        x1=st.text_input("请输入第二题的答案")
        if x1=="乘风破浪":
           st.write("Yes!!!😊")
           m=2
        else:
            st.write("No😭")
    if m==2:
        st.write('3.☀️☁️⚡')
        x1=st.text_input("请输入第三题的答案")
        if x1=="晴天霹雳":
           st.write("Yes!!!😊")
           m=3
        else:
            st.write("No😭")
    if m==3:
        st.write('4.🖐🌸⌚🚪')
        x1=st.text_input("请输入第四题的答案")
        if x1=="五花八门":
           st.write("Yes!!!😊")
           m=4
        else:
            st.write("No😭")
           
    if m==4:
        st.write('5.🌪️🍼🌊🐳')
        x1=st.text_input("请输入第五题的答案")
        if x1=="风平浪静":
           st.write("Yes!!!😊")
           m=5
           
        else:
            st.write("No😭")
    if m==5:
        st.write('你真棒！通过了所有的题目😉')
              
