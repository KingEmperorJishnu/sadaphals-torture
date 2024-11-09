import streamlit as st
st.set_page_config(layout="wide", page_title="Jishnu's Calculator", page_icon=":rocket:")
st.sidebar.title('Options')
j=st.sidebar.selectbox('What do you want to do?', 
['Calculate Volume', 'Calculate Surface Area'])
if (j=='Calculate Volume'):
  figure=st.selectbox(
'Select a figure',['Regular Pyramids','Cone','Cylinder','Sphere', 
'Regular prisms',])
  tab1, tab2=st.tabs(['Calculate volume', 'Inverse function'])
  with tab1:
    if (figure=='Regular Pyramids'):
      base=st.selectbox(
        'Select a base for the pyramid',['Square', 'Rectangle', 'Triangle'
,'Hexagon', 'Pentagon',])
      if (base=='Rectangle'):
        st.write('Volume of a rectangular pyramid')
        len_pyr=st.number_input('Enter the length of the base of the pyramid (in cm)')
        height_pyr=st.number_input('Enter the height of the pyramid (in cm)')
        width_pyr=st.number_input('Enter the width of the base of the pyramid (in cm)')
        st.write('Volume of the rectangular pyramid is',1/3*len_pyr*width_pyr*height_pyr
,' cm³')

      elif (base=='Square'):
        st.write('Volume of a square based pyramid')
        len_rec_pyr=st.number_input(
          'Enter the length of the base of the pyramid (in cm')
        height_rec_pyr=st.number_input('Enter the height of the pyramid (in cm)')
        st.write('The volume of the square based pyramid is',(1/3*len_rec_pyr**2*
height_rec_pyr),' cm³')

      elif (base=='Triangle'):
        st.write('Volume of a triangle based pyramid')
        len_tri_pyr=st.number_input("Enter the length of the pyramid's base (in cm)")
        height_tri_pyr=\
        st.number_input('Enter the height of the base of the pyramid (in cm)')
        Height_tri_pyramid=st.number_input('Enter the height of the pyramid (in cm)')
        st.write('The volume of the pyramid is',(1/3*len_tri_pyr*height_tri_pyr/2*
Height_tri_pyramid),' cm³')

      elif (base=='Hexagon'):
        st.write('Volume of a hexagonal pyramid')
        len_hex_pyr=\
        st.number_input('Enter the side length of the base of the pyramid (in cm)')
        height_hex_pyr=st.number_input('Enter the height of the pyramid (in cm)')
        st.write('The volume of the hexagonal pyramid is' ,(3**0.5/2*len_hex_pyr**2*
height_hex_pyr),' cm³')

      else:
        st.write('Volume of a pentagonal pyramid')
        len_pen_pyr=\
        st.number_input('Enter the side length of the base of the pyramid (in cm)')
        height_pen_pyr=st.number_input('Enter the height of the pyramid (in cm)')
        vol_pen_pyr=(5/12*height_pen_pyr*
len_pen_pyr**2*1.3764)
        st.write('The volume of the pentagonal pyramid is',vol_pen_pyr,' cm³')


    elif (figure=='Sphere'):
      st.write('Volume of a sphere')
      rad_sph=st.number_input('Enter the radius of the sphere (in cm)')
      st.write('Volume of the sphere is', (4/3*3.14*rad_sph**3), ' cm³')

    elif (figure=='Cone'):
      st.write('Volume of a cone')
      rad_cone=st.number_input('Enter the radius of the cone (in cm)')
      height_cone=st.number_input('Enter the height of the cone (in cm)')
      st.write('Volume of the cone is',(1/3*3.14*rad_cone**2*height_cone),' cm³')

    elif (figure=='Cylinder'):
      st.write('Volume of a cylinder')
      rad_cyl=st.number_input('Enter the radius of the cylinder (in cm)')
      height_cyl=st.number_input('Enter the height of the cylinder (in cm)')
      st.write('Volume of the cylinder is',(3.14*rad_cyl**2*height_cyl),' cm³')

    elif(figure=='Regular prisms'):
      choice=st.selectbox('Select a base for a prism', [
'Rectangle',
'Triangle',
'Hexagon',
'Pentagon'])
      if (choice=='Rectangle'):
        st.write('Volume of a rectangular prism')
        len_rp=st.number_input('Enter the length of the rectangular prism (in cm)')
        width_rp=st.number_input('Enter the width of the rectangular prism (in cm)')
        height_rp=st.number_input('Enter the height of the rectangular prism (in cm)')
        st.write('Volume of the rectangular prism is',len_rp*width_rp*height_rp,' cm³')

      elif (choice=='Triangle'):
        st.write('Volume of a triangular prism')
        len_tp=st.number_input('Enter the length of the base of the prism (in cm)')
        height_tp=st.number_input('Enter the height of the base of the prism (in cm)')
        Height_tp=st.number_input('Enter the height of the triangular prism (in cm)')
        st.write('Volume of the rectangular prism is',(len_tp*height_tp/2*Height_tp),
' cm³')


      elif (choice=='Hexagon'):
        st.write('Volume of a hexagonal prism')
        len_hp=st.number_input('Enter the side length of the base of the prism (in cm)')
        height_hp=st.number_input('Enter the height of the hexagonal prism (in cm)')
        st.write('Volume of the rectangular prism is',(3*3**0.5/2*len_hp**2*height_hp),
' cm³')



      else:
        st.write('Volume of a pentagonal prism')
        len_pp=st.number_input('Enter the side length of the pentagonal prism (in cm)')
        height_pp=st.number_input('Enter the height of the pentagonal prism (in cm)')
        vol_pen_pyr=(5/12*height_pp*len_pp**2*1.3764)
        vol_pp=(vol_pen_pyr*3)
        st.write('Volume of the rectangular prism is',vol_pp,' cm³')

  with tab2:
    
    if (figure=='Sphere'):
      rad_dia=st.selectbox('What would you like to find',['Radius','Diameter'])
      if (rad_dia=='Radius'):
        vol_rad=st.number_input('Enter the volume of the sphere (in cm³)')
        if (vol_rad==0):
          st.write('Volume must exceed 0')
        rad=(vol_rad*(3/4)/3.1415)**(1/3)
        st.write('The radius of the sphere is ',rad,' cm')
      else:
        vol_dia=st.number_input('Enter the volume of the sphere (in cm³)')
        dia=((vol_dia*(3/4)/3.1415)**(1/3))*2
        st.write('The radius of the sphere is ',dia,' cm')

    elif (figure=='Cone'):
      cone_choice=st.selectbox(
        'What would you like to find?',[
          'Radius of the base','Height','Diameter of the base'])
      if (cone_choice=='Height'):
        cone_rad=st.number_input('Enter the radius of the base of the cone (in cm)')
        cone_vol=st.number_input('Enter the volume of the cone (in cm³)')
        if (cone_vol==0):
          st.write('The volume must exceed 0')
        else:
          thing1=(3.1415*cone_rad**2)
          if thing1!=0:
            height=(cone_vol*(1/thing1)*3)
            st.write('The height of the cone is ',height,' cm')
          else:
            st.write('Radius must exceed 0')
      elif (cone_choice=='Radius of the base'):
        cone_vol1=st.number_input('Enter the volume of the cone (in cm³)')
        height_cone=st.number_input(
          'Enter the height of the cone (in cm)',key='height_input')
        if (height_cone==0 or cone_vol1==0):
          st.write('The volume and height must exceed 0')
        else:
          len_rad=(3*(cone_vol1/(3.1415*height_cone)))**0.5
          st.write('The radius of the base of the cone is ',len_rad,' cm')
      else:
        cone_vol2=st.number_input('Enter the volume of the cone (in cm³)')
        height_cone2=st.number_input(
          'Enter the height of the cone (in cm)',key='height_input')
        if (height_cone2==0 or cone_vol2==0):
          st.write('The volume and height must exceed 0')
        else:
          len_rad=((3*(cone_vol2/(3.1415*height_cone2)))**0.5)*2
          st.write('The diameter of the base of the cone is ',len_rad,' cm')

    elif (figure=='Cylinder'):
      cyl_choice=st.selectbox(
        'What would you like to find?',[
          'Radius','Height','Diameter'])
      if (cyl_choice=='Radius'):
        cyl_vol=st.number_input('Enter the volume of the cylinder (in cm³)')
        cyl_height=st.number_input(
          'Enter the height of the cylinder (in cm)', key='height2')
        if (cyl_vol==0 or cyl_height==0):
          st.write('The volume and height must exceed 0')
        else:
          rad_cyl=(cyl_vol/(3.1415*cyl_height))**0.5
          st.write('The radius of the cylinder is ',rad_cyl,' cm')

      elif (cyl_choice=='Height'):
        cyl_vol3=st.number_input('Enter the volume of the cylinder (in cm³)')
        cyl_rad4=st.number_input(
          'Enter the radius of the cylinder (in cm)',key='radius')
        if (cyl_vol3==0 or cyl_rad4==0):
          st.write('The volume and radius must exceed 0')
        else:
          height_cyl=(cyl_vol3/(3.1415*(cyl_rad4)**2))
          st.write('The height of the cylinder is ',height_cyl,' cm')
      else:
        cyl_vol5=st.number_input('Enter the volume of the cylinder (in cm³)')
        cyl_height5=st.number_input('Enter the height of the cylinder (in cm)', key='height3')
        if (cyl_vol5==0 or cyl_height5==0):
          st.write('The volume and height must exceed 0')
        else:
          dia_cyl=((cyl_vol5/(3.1415*cyl_height5))**0.5)*2
          st.write('The diameter of the cylinder is ',dia_cyl,' cm')

    elif (figure=='Regular Pyramids'):
      base_choice=st.selectbox(
        'Select a base for the pyramid',[
          'Square', 'Rectangle', 'Triangle','Pentagon','Hexagon'])
      if (base_choice=='Rectangle'):
        dimension=st.selectbox('What would you like to find?',[
          'Length','Width','Height'])
        if (dimension=='Length'):
          vol_tpyr4=st.number_input('Enter the volume of the pyramid (in cm³)')
          height_tpyr4=st.number_input(
            'Enter the height of the pyramid (in cm)', key='height45')
          width_tpyr4=st.number_input(
            'Enter the width of the base of the pyramid (in cm)',key='witdhtpyr')
          if (vol_tpyr4==0 or height_tpyr4==0 or width_tpyr4==0):
            st.write('The volume, height and width must exceed 0')
          else:
            len_tpyr=(3*vol_tpyr4/(height_tpyr4*width_tpyr4))
            st.write('The length of the base of the pyramid is ',len_tpyr,' cm')

        elif (dimension=='Width'):
          vol_tpyr4=st.number_input('Enter the volume of the pyramid (in cm³)')
          height_tpyr5=st.number_input(
            'Enter the height of the pyramid (in cm)', key='height46')
          length_tpyr5=st.number_input(
            'Enter the length of the base of the pyramid (in cm)')
          if (vol_tpyr4==0 or height_tpyr5==0 or length_tpyr5==0):
            st.write('The volume, height and width must exceed 0')
          else:
            wid_tpyr=(3*vol_tpyr4/(height_tpyr5*length_tpyr5))
            st.write('The length of the base of the pyramid is ',wid_tpyr,' cm')

        else:
            vol_tpyr6=st.number_input('Enter the volume of the pyramid (in cm³)')
            len_tpyr9=st.number_input(
              'Enter the length of the pyramid (in cm)', key='length48')
            width_tpyr6=st.number_input(
              'Enter the width of the base of the pyramid (in cm)')
            if (vol_tpyr6==0 or len_tpyr9==0 or width_tpyr6==0):
              st.write('The volume, height and width must exceed 0')
            else:
              height_tpyr=(3*vol_tpyr6/(len_tpyr9*width_tpyr6))
              st.write('The length of the base of the pyramid is ',height_tpyr,' cm')

      elif (base_choice=='Square'):
        dimensions=st.selectbox('What would you like to find?',[
            'Side length','Height'])
        if (dimensions=='Side length'):
          vol_tpyr10=st.number_input('Enter the volume of the pyramid (in cm³)')
          height_tpyr10=st.number_input(
              'Enter the height of the pyramid (in cm)', key='height50')
          if (vol_tpyr10==0 or height_tpyr10==0):
            st.write('Volume and height must exceed 0')
          else:
            len_sqr=(3*(vol_tpyr10/height_tpyr10))**0.5
            st.write('The side length of the base of the pyramid is', len_sqr,' cm')

        else:
          vol_tpyr11=st.number_input('Enter the volume of the pyramid (in cm³)')
          sid_len=st.number_input(
              'Enter the side length of the pyramid (in cm)', key='side50')
          if (vol_tpyr11==0 or sid_len==0):
            st.write('Volume and side length must exceed 0')
          else:
            height_sqr=(3*(vol_tpyr11/(sid_len**2)))
            st.write('The side length of the base of the pyramid is', height_sqr,' cm')

      elif (base_choice=='Triangle'):
        dimension_tri=st.selectbox('What would you like to find?',[
            'Length','Height','Height of the base'])
        if (dimension_tri=='Length'):
          vol_tpyr12=st.number_input('Enter the volume of the pyramid (in cm³)')
          height_tpyr12=st.number_input(
              'Enter the height of the pyramid (in cm)', key='height51')
          height_tpyr13=st.number_input(
              'Enter the height of the base of the pyramid (in cm)', key='height52')
          if (vol_tpyr12==0 or height_tpyr12==0 or height_tpyr13==0):
            st.write('Volume, height and height of the base must exceed 0')
          else:
            len_tri=(3*vol_tpyr12/(height_tpyr12*(height_tpyr13/2)))
            st.write('The length of the base of the pyramid is', len_tri,' cm')

        elif (dimension_tri=='Height'):
          vol_tripyr=st.number_input('Enter the volume of the pyramid (in cm³)')
          len_tripyr=st.number_input(
            'Enter the length of the base of the pyramid (in cm)')
          bs_height=st.number_input(
            'Enter the height of the base of the pyramid (in cm)', key='height60')
          if (vol_tripyr==0 or len_tripyr==0 or bs_height==0):
            st.write('Volume, length and height of the base must exceed 0')
          else:
            HHeight=(3*vol_tripyr/(len_tripyr*bs_height/2))
            st.write('The height of the pyramid is ', HHeight,' cm')

        else:
          vol_123456789=st.number_input('Enter the volume of the pyramid (in cm³)')
          len_123456789=st.number_input(
            'Enter the length of the base of the pyramid (in cm)')
          height_123456789=st.number_input(
            'Enter the height of the pyramid (in cm)', key='height61')
          if (vol_123456789==0 or len_123456789==0 or height_123456789==0):
            st.write('Volume, length and height must exceed 0')
          else:
            bs_height123=(3*vol_123456789/(len_123456789*height_123456789/2))
            st.write('The height of the base of the pyramid is ', bs_height123,' cm')

      
      
      elif (base_choice=='Hexagon'):
        dimension_hex23=st.selectbox('What would you like to find?',[
          'Side Length','Height'])
        if (dimension_hex23=='Height'):
          volume=st.number_input('Enter the volume of the pyramid (in cm³)')
          side_length222=st.number_input(
            "Enter the side length of the pyramid's base (in cm)", key='side425')
          if (volume==0 or side_length222==0):
            st.write('Volume and height must exceed 0')
          else:
            heightxx=(3*volume/(2.59807*(side_length222**2)))
            st.write('The height of the base of the pyramid is', heightxx,' cm')

        elif (dimension_hex23=='Side Length'):
          vol_tpyr19=st.number_input('Enter the volume of the pyramid (in cm³)')
          height_tpyr19=st.number_input(
            'Enter the height of the pyramid (in cm)', key='height415')
          if (vol_tpyr19==0 or height_tpyr19==0):
            st.write('Volume and height must exceed 0')
          else:
            hexside8=  (vol_tpyr19*3/(2.59807*height_tpyr19))**0.5
            st.write('The side length of the base of the prism is', hexside8,' cm')
      
      
      elif (base_choice=='Pentagon'):
        
          dimension_pent=st.selectbox('What would you like to find?',[
              'Side Length','Height'])
          if (dimension_pent=='Side Length'):
            vol_penta=st.number_input('Enter the volume of the pyramid (in cm³)')
            height_penta=st.number_input(
              'Enter the height of the pyramid (in cm)',key='Height of the pyramid')
            if (vol_penta==0 or height_penta==0):
              st.write('The volume and the heigth must exceed 0')
            else:
              sidpentleng=((3*vol_penta)/(1.7204774*height_penta))**0.5
              st.write(
                'The side length of the base of the pyramid is', sidpentleng,' cm')

          else:
            vol_pent12=st.number_input('Enter the volume of the pyramid (in cm³)')
            side_length12=st.number_input(
                'Enter the side length of the pyramid (in cm)', key='side435')
            if (vol_pent12==0 or side_length12==0):
              st.write('Volume and side length must exceed 0')
            else:
              heightpentpyr=((3*vol_pent12)/(1.7204774*(side_length12**2)))
              st.write('The height of the pyramid is', heightpentpyr,' cm')
      
          
          
    elif (figure=='Regular prisms'):
      base_choice=st.selectbox(
        'Select a base for the prism',[
          'Rectangle', 'Triangle','Pentagon','Hexagon'])
      if (base_choice=='Rectangle'):
        dimension0=st.selectbox('What would you like to find?',[
          'Length','Width','Height'])
        if (dimension0=='Length'):
          vol_tpyr41=st.number_input('Enter the volume of the prism (in cm³)')
          height_tpyr41=st.number_input(
            'Enter the height of the prism (in cm)', key='height45')
          width_tpyr41=st.number_input(
            'Enter the width of the base of the prism (in cm)')
          if (vol_tpyr41==0 or height_tpyr41==0 or width_tpyr41==0):
            st.write('The volume, height and width must exceed 0')
          else:
            len_tpr=(vol_tpyr41/(height_tpyr41*width_tpyr41))
            st.write('The length of the base of the prism is ',len_tpr,' cm')

        elif (dimension0=='Width'):
          vol_tpyr51=st.number_input('Enter the volume of the prism (in cm³)')
          height_tpyr51=st.number_input(
            'Enter the height of the prism (in cm)', key='height4040')
          length_tpyr51=st.number_input(
            'Enter the length of the base of the prism (in cm)',key='Length')
          if (vol_tpyr51==0 or height_tpyr51==0 or length_tpyr51==0):
            st.write('The volume, height and width must exceed 0')
          else:
            wid_tpyr51=(vol_tpyr51/(height_tpyr51*length_tpyr51))
            st.write('The length of the base of the prism is ',wid_tpyr51,' cm')

        else:
            vol_tpyr60=st.number_input('Enter the volume of the prism (in cm³)')
            len_tpyr90=st.number_input(
              'Enter the length of the prism (in cm)', key='length58')
            width_tpyr60=st.number_input(
              'Enter the width of the base of the prism (in cm)')
            if (vol_tpyr60==0 or len_tpyr90==0 or width_tpyr60==0):
              st.write('The volume, height and width must exceed 0')
            else:
              height_tpyr0=(vol_tpyr60/(len_tpyr90*width_tpyr60))
              st.write('The length of the base of the prism is ',height_tpyr0,' cm')
              

      

      elif (base_choice=='Triangle'):
        dimension_trip=st.selectbox('What would you like to find?',[
            'Length','Height','Height of the base'])
        if (dimension_trip=='Length'):
          vol_tpyr15=st.number_input('Enter the volume of the prism (in cm³)')
          height_tpyr15=st.number_input(
              'Enter the height of the prism (in cm)', key='height512')
          height_tpyr15=st.number_input(
              'Enter the height of the base of the prism (in cm)', key='height522')
          if (vol_tpyr15==0 or height_tpyr15==0 or height_tpyr15==0):
            st.write('Volume, height and height of the base must exceed 0')
          else:
            len_tri=(vol_tpyr15/(height_tpyr15*(height_tpyr15/2)))
            st.write('The length of the base of the prism is', len_tri,' cm')

        elif (dimension_trip=='Height'):
          vol_tripr=st.number_input('Enter the volume of the prism (in cm³)')
          len_tripr=st.number_input(
            'Enter the length of the base of the prism (in cm)')
          bs_11height=st.number_input(
            'Enter the height of the base of the prism (in cm)', key='height61')
          if (vol_tripr==0 or len_tripr==0 or bs_11height==0):
            st.write('Volume, length and height of the base must exceed 0')
          else:
            HHeight=(3*vol_tripr/(len_tripr*bs_11height/2))
            st.write('The height of the prism is ', HHeight,' cm')

        else:
          vol_12345689=st.number_input('Enter the volume of the prism (in cm³)')
          len_12345689=st.number_input(
            'Enter the length of the base of the prism (in cm)')
          height_12345689=st.number_input(
            'Enter the height of the prism (in cm)', key='height64')
          if (vol_12345689==0 or len_12345689==0 or height_12345689==0):
            st.write('Volume, length and height must exceed 0')
          else:
            bs_height1223=(vol_12345689/(len_12345689*height_12345689/2))
            st.write('The height of the base of the pyramid is ', bs_height1223,' cm')

      elif (base_choice=='Hexagon'):
        dimension_hex=st.selectbox('What would you like to find?',[
            'Side Length','Height'])
        if (dimension_hex=='Height'):
          vol_tpyr16=st.number_input('Enter the volume of the prism (in cm³)')
          side_length22=st.number_input(
              'Enter the side length of the prism (in cm)', key='side45')
          if (vol_tpyr16==0 or side_length22==0):
            st.write('Volume and height must exceed 0')
          else:
            heightxx=(vol_tpyr16/(2.59807*(side_length22**2)))
            st.write('The side length of the base of the prism is', heightxx,' cm')

        elif (dimension_hex=='Side Length'):
          vol_tpyr17=st.number_input('Enter the volume of the prism (in cm³)')
          height_tpyr17=st.number_input(
              'Enter the height of the prism (in cm)', key='height405')
          if (vol_tpyr17==0 or height_tpyr17==0):
            st.write('Volume and height must exceed 0')
          else:
            hexside=(vol_tpyr17/(2.59807*height_tpyr17))**0.5
            st.write('The side length of the base of the prism is', hexside,' cm')

    
      elif (base_choice=='Pentagon'):
        dimension_pent=st.selectbox('What would you like to find?',[
            'Length','Height'])
        if (dimension_pent=='Length'):
          vol_pent=st.number_input('Enter the volume of the prism (in cm³)')
          height_pent=st.number_input('Enter the height of the prism (in cm)')
          if (vol_pent==0 or height_pent==0):
            st.write('The volume and the heigth must exceed 0')
          else:
            sidpentlen=(vol_pent/(1.7204774*height_pent))**0.5
            st.write('The side length of the base of the prism is', sidpentlen,' cm')

        else:
          vol_pent2=st.number_input('Enter the volume of the prism (in cm³)')
          side_length2=st.number_input(
              'Enter the side length of the prism (in cm)', key='side45')
          if (vol_pent2==0 or side_length2==0):
            st.write('Volume and side length must exceed 0')
          else:
            heightpent=(vol_pent2/(1.7204774*(side_length2**2)))
            st.write('The height of the base of the prism is', heightpent,' cm')
        
        


elif (j=='Calculate Surface Area'):
  surface_figure=st.selectbox(
'Select a figure',['Regular Pyramids','Cone','Cylinder','Sphere', 
'Regular Prisms',])
  tab3,tab4=st.tabs(['Surface Area Calculator','Inverse function'])
  with tab3:
    if (surface_figure=='Regular Prisms'):
      surface_choice=st.selectbox('Select a base for a prism', [
'Rectangle',
'Triangle',
'Hexagon',
'Pentagon'])

      if (surface_choice=='Rectangle'):
        st.write('Surface area of a rectangular prism')
        len_rp_surface=st.number_input('Enter the base length of the prism (in cm)')
        width_rp_surface=st.number_input(
        'Enter the width of the base of the prism(in cm)')
        height_rp_surface=st.number_input('Enter the height of the prism (in cm)')
        sa_rp=(2*(len_rp_surface*width_rp_surface+len_rp_surface*height_rp_surface+width_rp_surface*height_rp_surface))
        st.write('The surface area of this prism is',sa_rp,'cm²')

      elif (surface_choice=='Triangle'):
        st.write('Surface area of a triangular prism')
        len_tp_surface=st.number_input('Enter the base length of the prism (in cm)')
        width_tp_surface=st.number_input(
        'Enter the height of the base of the prism(in cm)')
        height_tp_surface=st.number_input('Enter the height of the prism (in cm)')
        sa_tp=(2*(len_tp_surface*width_tp_surface/2+len_tp_surface*height_tp_surface+width_tp_surface*height_tp_surface))
        st.write('The surface area of this prism is',sa_tp,'cm²')

      elif (surface_choice=='Hexagon'):
        st.write('Surface area of a hexagonal prism')
        len_hp_surface=st.number_input('Enter the base length of the prism (in cm)')
        height_hp_surface=st.number_input('Enter the height of the prism (in cm)')
        sa_hp=(6*len_hp_surface*height_hp_surface+3*3**0.5*len_hp_surface**2)
        st.write('The surface area of this prism is',sa_hp,'cm²')

      elif (surface_choice=='Pentagon'):
        st.write('Surface area of a pentagonal prism')
        len_pp_surface=st.number_input('Enter the base length of the prism(in cm)')
        height_pp_surface=st.number_input('Enter the height of the prism (in cm)')
        sa_pp=(5*len_pp_surface*height_pp_surface)+((1/2*(5*(5+(2*5**0.5)))**0.5)*len_pp_surface**2)
      #((1/2*(5*(5+(2*5**0.5)))**0.5 that part is equal to 3.440954
        st.write('The surface area of this prism is',sa_pp,'cm²')


    elif (surface_figure=='Sphere'):
      st.write('Surface area of a sphere')
      rad_sph_surface=st.number_input('Enter the radius of the sphere (in cm)')
      sa_sph=(4*3.14*rad_sph_surface**2)
      st.write('Surface area of the sphere is',sa_sph,'cm²')

  
    elif (surface_figure=='Cylinder'):    
      st.write('Surface area of a cylinder')
      rad_cyl_surface=st.number_input('Enter the radius of the cylinder (in cm)')
      height_cyl_surface=st.number_input('Enter the height of the cylinder (in cm)')
      sa_cyl=(2*3.14*rad_cyl_surface**2)+(2*3.14*rad_cyl_surface*height_cyl_surface)
      st.write('Surface area of the cylinder is',sa_cyl,'cm²')

    elif (surface_figure=='Cone'):
      st.write('Surface area of a cone')
      rad_cone_surface=st.number_input('Enter the radius of the cone (in cm)')
      height_cone_surface=st.number_input('Enter the height of the cone (in cm)')
      diagonal=(rad_cone_surface**2+height_cone_surface**2)**0.5
      sa_cone=(3.14*rad_cone_surface**2+3.14*rad_cone_surface*diagonal)
      st.write('Surface area of the cone is',sa_cone,'cm²')

    elif (surface_figure=='Regular Pyramids'):
      sur_pyr_choice=st.selectbox('Select a base for a pyramid' ,[
'Rectangle',
'Triangle',
'Hexagon',
'Pentagon'])
      if (sur_pyr_choice=='Rectangle'):
        st.write('Surface area of a rectangular pyramid')
        len_rpyr_surface=st.number_input('Enter the base length of the pyramid (in cm)')
        width_rpyr_surface=st.number_input(
        'Enter the width of the base of the pyramid (in cm)')
        height_rpyr_surface=st.number_input('Enter the height of the pyramid (in cm)')
        diagonal_rpyr_sur1=((len_rpyr_surface/2)**2+(width_rpyr_surface**2))**0.5
        diagonal_rpyr_sur2=((width_rpyr_surface/2)**2+(len_rpyr_surface**2))**0.5
        sa_rp_pyr=(len_rpyr_surface*width_rpyr_surface)+(len_rpyr_surface*diagonal_rpyr_sur2)+(width_rpyr_surface*diagonal_rpyr_sur1)
        st.write('The surface area of this pyramid is ',sa_rp_pyr,' cm²')

      elif (sur_pyr_choice=='Triangle'):
        st.write(
          'Surface area of regular triangular pyramid (base is an equilateral triangle)')
        len_tpyr_surface=st.number_input('Enter the side length of the base (in cm)')
        height_tpyr_surface=st.number_input(
        'Enter the height of the pyramid of the pyramid (in cm)')
        baseheight=((len_tpyr_surface**2)-((len_tpyr_surface/2)**2))**0.5
        slant=(((baseheight/2)**2)+((height_tpyr_surface)**2))**0.5
        sa_tpyr=(slant*3*len_tpyr_surface)+((len_tpyr_surface*baseheight)/2)
        st.write('The surface area of this pyramid is', sa_tpyr,' cm²')

      elif (sur_pyr_choice=='Hexagon'):
        st.write('Surface area of a hexagonal pyramid')
        len_hpyr_surface=st.number_input('Enter the side length of the base (in cm)')
        height_hpyr_surface=st.number_input(
        'Enter the height of the pyramid of the pyramid (in cm)')
        sa_hpyr=((3*(3**0.5))/2)*(len_hpyr_surface**2)+(3*len_hpyr_surface)*(((height_hpyr_surface**2)+(3*len_hpyr_surface**2)/4)**0.5)
        st.write('The surface area of this pyramid is', sa_hpyr,' cm²')

      else:
        st.write('Surface area of a pentagonal pyramid')
        len_ppyr_surface=st.number_input('Enter the side length of the base (in cm)')
        height_ppyr_surface=st.number_input('Enter the height of the base (in cm)')
        if (len_ppyr_surface==0 or height_ppyr_surface==0):
          st.write('The length of the base and the height must be greater than 0')
        else:
          p1=(5/4)*1.37638*(len_ppyr_surface**2)
          p2=5*(len_ppyr_surface/2)
          p3=((height_ppyr_surface**2)+(len_ppyr_surface*1.37638/2)**2)**0.5
          sa_ppyr=p1+(p2*p3)
          st.write('The surface area of this pyramid is', sa_ppyr,' cm²')

  with tab4:
    if (surface_figure=='Sphere'):
      radia=st.selectbox('What would you like to find?',['Radius', 'Diameter'])
      if (radia=='Radius'):
        sa=st.number_input('Enter the surface area of the sphere (in cm²)')
        rad_sph_inv=((sa/(4*3.14159))**0.5)
        st.write('The radius of the sphere is',rad_sph_inv,' cm')
      else:
        sa2=st.number_input('Enter the surface area of the sphere (in cm²)')
        dia_sph_inv=((sa2/(4*3.14159))**0.5)*2
        st.write('The diameter of the sphere is',dia_sph_inv,' cm')

    if (surface_figure== 'Cylinder'):
      radiaheight=st.selectbox(
        'What would you like to find?',['Radius', 'Height','Diameter'])
      if (radiaheight=='Height'):
        sa3=st.number_input('Enter the surface area of the cylinder (in cm²)')
        rad22=st.number_input(
          'Enter the radius of the cylinder (in cm)',key='radius 22')
        if (sa3<=0 or rad22<=0):
          st.write('The surface area and the radius must be greater than 0')
        else:
          height_cyl_inv=(sa3/(2*3.14159*rad22)-rad22)
          st.write('The height of the cylinder is',height_cyl_inv,' cm')
      
      elif (radiaheight=='Radius'):
        sa4=st.number_input('Enter the surface area of the cylinder (in cm²)')
        Height24=st.number_input(
          'Enter the height of the cylinder (in cm)',key='height24')
        rad_cyl_inv=(1/2)*((Height24**2+(2*sa4/3.14159))**0.5)-(Height24/2)
        st.write('The height of the cylinder is',rad_cyl_inv,' cm')
      else:
        sa5=st.number_input('Enter the surface area of the cylinder (in cm²)')
        Height25=st.number_input(
          'Enter the height of the cylinder (in cm)',key='height25')
        dia_cyl_inv=((1/2)*((Height25**2+(2*sa5/3.14159))**0.5)-(Height25/2))*2
        st.write('The height of the cylinder is',dia_cyl_inv,' cm')

    elif (surface_figure=='Cone'):
      cone_choice=st.selectbox(
        'What would you like to find?',[
          'Radius of the base','Height','Diameter of the base'])
      if (cone_choice=='Radius of the base'):
        sa_cone_inv=st.number_input('Enter the surface area of the cone (in cm²)')
        height_cone_inv=st.number_input(
          'Enter the height of the cone (in cm)',key='height_cone123')
        if (sa_cone_inv<=0 or height_cone_inv<=0):
          st.write('The surface area and the height must be greater than 0')
        else:
          p1=(sa_cone_inv**2)
          p2=3.14159*(3.14159*(height_cone_inv**2)+(2*sa_cone_inv))
          rad_cone_inv=(p1/p2)**0.5
          st.write('The radius of the base of the cone is',rad_cone_inv,' cm')

      elif (cone_choice=='Height'):
        sa_cone1=st.number_input('Enter the surface area of the cone (in cm²)')
        rad123=st.number_input('Enter the radius of the base of the cone (in cm)')
        if (sa_cone1<=0 or rad123<=0):
          st.write('The surface area and the radius must be greater than 0')
        else:
          if (sa_cone1<(2*3.14159*(rad123**2))):
            st.write('The surface area must be greater than 2*pi*r²')
          else:
            p1=(sa_cone1*((sa_cone1/(rad123**2))-(2*3.14159)))
            height_cone_inv_calc=((p1)**0.5)/3.14159
            st.write('The height of the cone is ',height_cone_inv_calc,' cm')

    elif (surface_figure=='Regular Pyramids'):
      st.write('Inverse function for hexagonal pyramid')
      pyr_choice='Hexagon'
      if (pyr_choice=='Hexagon'):
        choicechoice=st.selectbox(
          'What would you like to find?',['Height','Side Length'])
        if (choicechoice=='Height'):
          sa_pyr_inv=st.number_input('Enter the surface area of the pyramid (in cm²)')
          side_length_pyr_inv=st.number_input(
            'Enter the side length of the base of the pyramid (in cm)')
          if (sa_pyr_inv<=0 or side_length_pyr_inv<=0):
            st.write('The surface area and the side length must be greater than 0')
          else:
            height_pyr_inv=(1/3)*(((sa_pyr_inv*(sa_pyr_inv/(side_length_pyr_inv**2))-(27**0.5)))**0.5)
            st.write('The height of the pyramid is',height_pyr_inv,' cm')

        else:
          sa_input_hex=st.number_input('Enter the surface area of the pyramid (in cm²)')
          height_input_hex=st.number_input(
            'Enter the height of the pyramid (in cm)',key='hexagon_inv_height')
          if (sa_input_hex<=0 or height_input_hex<=0):
            st.write('Surface area and height must exceed 0')
          else:
            p1=sa_input_hex**2
            p2=3*((3*(height_input_hex**2))+((sa_input_hex*3)**0.5))
            sl_hex=(p1/p2)**0.5
            st.write('The side length of the base of the pyramid is',sl_hex,' cm')


    elif (surface_figure=='Regular Prisms'):
      st.write('Inverse function for rectangular prism')
      prism_choice='Rectangle'
      findwhat=st.selectbox(
        'What would you like to find?',['Height','Length','Width'])
      if (findwhat=='Height'):
        sa_rp_inv=st.number_input('Enter the surface area of the prism (in cm²)')
        len=st.number_input(
          'Enter the length of the base of the prism (in cm)')
        w=st.number_input(
          'Enter the width of the base of the prism (in cm)')
        if (sa_rp_inv<=0 or len<=0 or w<=0):
          st.write('The surface area, length and width must be greater than 0')
        else:
         height_rp_inv=((sa_rp_inv/2)-(len*w))/(len+w)
         if (height_rp_inv<=0):
           st.write('Invalid input')
         else:
          st.write('The height of the prism is',height_rp_inv,' cm')

      elif (findwhat=='Length'):
        sa_rp1_inv=st.number_input('Enter the surface area of the prism (in cm²)')
        h=st.number_input(
          'Enter the height of the base of the prism (in cm)')
        w=st.number_input(
          'Enter the width of the base of the prism (in cm)')
        if (sa_rp1_inv<=0 or h<=0 or w<=0):
          st.write('The surface area, length and width must be greater than 0')
        else:
         len234=((sa_rp1_inv/2)-(h*w))/(h+w)
         if (len234<=0):
           st.write('Invalid input')
         else:
          st.write('The height of the prism is',len234,' cm')

      if (findwhat=='Width'):
        sa_rp3_inv=st.number_input('Enter the surface area of the prism (in cm²)')
        len=st.number_input(
          'Enter the length of the base of the prism (in cm)')
        h=st.number_input(
          'Enter the height of the base of the prism (in cm)')
        if (sa_rp3_inv<=0 or len<=0 or h<=0):
          st.write('The surface area, length and width must be greater than 0')
        else:
         width=((sa_rp3_inv/2)-(len*h))/(len+h)
         if (width<=0):
           st.write('Invalid input')
         else:
          st.write('The height of the prism is',width,' cm')
        

          

