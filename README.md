# Assignment-1-Rectangle

 public void GetRectangleLength_input7_expectedLengthEquals7()
        {
            //Arrange
            int l = 7;
            int w = 6;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int length = test.GetRectangleLength();
            //Assert
            Assert.AreEqual(l, length);
        }
