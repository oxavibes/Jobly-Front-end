<template>
  <form action="#" class="dashboard-form job-post-form">
    <div class="dashboard-section basic-info-input">
      <h4><i data-feather="user-check"></i>Post A Job</h4>
      <div class="form-group row">
        <label class="col-md-3 col-form-label">Job Title</label>
        <div class="col-md-9">
          <input
            type="text"
            class="form-control"
            placeholder="Your job title here"
          />
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Job Summery</label>
        <div class="col-md-9">
          <div class="row">
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Select Category</option>
                  <option>Accounting / Finance</option>
                  <option>Health Care</option>
                  <option>Garments / Textile</option>
                  <option>Telecommunication</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Job Location"
                />
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Job Type</option>
                  <option>Part Time</option>
                  <option>Full Time</option>
                  <option>Temperory</option>
                  <option>Permanent</option>
                  <option>Freelance</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Experience (Optional)</option>
                  <option>Less than 1 Year</option>
                  <option>2 Year</option>
                  <option>3 Year</option>
                  <option>4 Year</option>
                  <option>Over 5 Year</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Salary Range"
                />
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Qualification</option>
                  <option>Matriculation</option>
                  <option>Intermidiate</option>
                  <option>Gradute</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Gender</option>
                  <option>Male</option>
                  <option>Female</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <input type="text" class="form-control" placeholder="Vacancy" />
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group datepicker">
                <input type="date" class="form-control" />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Job Description</label>
        <div class="col-md-9">
          <textarea
            id="mytextarea"
            class="tinymce-editor tinymce-editor-1"
            placeholder="Description text here"
          ></textarea>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Responsibilities</label>
        <div class="col-md-9">
          <textarea
            id="mytextarea2"
            class="tinymce-editor tinymce-editor-2"
            placeholder="Responsibilities (Optional)"
          ></textarea>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Education</label>
        <div class="col-md-9">
          <textarea
            id="mytextarea3"
            class="tinymce-editor tinymce-editor-2"
            placeholder="Education (Optional)"
          ></textarea>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Other Benefits</label>
        <div class="col-md-9">
          <textarea
            id="mytextarea4"
            class="tinymce-editor tinymce-editor-2"
            placeholder="Description text here"
          ></textarea>
        </div>
      </div>
      <div class="form-group row">
        <label class="col-md-3 col-form-label">Your Location</label>
        <div class="col-md-9">
          <div class="row">
            <div class="col-md-6">
              <div class="form-group">
                <select class="form-control">
                  <option>Country</option>
                  <option>USA</option>
                  <option>United Kindom</option>
                  <option>Spain</option>
                  <option>France</option>
                  <option>Germany</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
              <div class="form-group">
                <select class="form-control" id="exampleFormControlSelect11">
                  <option>City</option>
                  <option>New Work</option>
                  <option>Washington D.C</option>
                  <option>California</option>
                  <option>Las Vegas</option>
                </select>
                <i class="fa fa-caret-down"></i>
              </div>
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Zip Code"
                />
              </div>
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Your Location"
                />
              </div>
            </div>
            <div class="col-md-6">
              <div class="set-location">
                <h5>Pin Location</h5>
                <div id="map-area" class="contact-location">
                  <div
                    class="cp-map"
                    id="location"
                    data-lat="40.713355"
                    data-lng="-74.005535"
                    data-zoom="10"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">About Company</label>
        <div class="col-md-9">
          <div class="row">
            <div class="col-md-6">
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Company Name"
                />
              </div>
            </div>
            <div class="col-md-6">
              <div class="form-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Web Address"
                />
              </div>
            </div>
            <div class="col-md-12">
              <div class="form-group">
                <textarea
                  class="form-control"
                  placeholder="Company Profile"
                ></textarea>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <label class="col-md-3 col-form-label">Select Package</label>
        <div class="col-md-9">
          <div class="package-select">
            <div class="package-select-inputs">
              <div class="form-group">
                <input
                  class="custom-radio"
                  type="radio"
                  id="radio_1"
                  name="my-radio"
                  value="1"
                  checked
                />
                <label for="radio_1">
                  <span class="dot"></span>
                  <span class="package-type">Free</span> $0.00
                </label>
              </div>
              <div class="form-group">
                <input
                  class="custom-radio"
                  type="radio"
                  id="radio_2"
                  name="my-radio"
                  value="1"
                />
                <label for="radio_2">
                  <span class="dot"></span>
                  <span class="package-type">Stater</span> $22.00
                </label>
              </div>
              <div class="form-group">
                <input
                  class="custom-radio"
                  type="radio"
                  id="radio_3"
                  name="my-radio"
                  value="1"
                />
                <label for="radio_3">
                  <span class="dot"></span>
                  <span class="package-type">Advance</span> $44.00
                </label>
              </div>
            </div>
            <div class="payment-method">
              <a href="#" class="credit active"
                ><i class="fas fa-credit-card"></i>Credit Card</a
              >
              <a href="#" class="paypal"
                ><i class="fab fa-cc-paypal"></i>PayPal</a
              >
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-9 offset-md-3">
          <div class="form-group terms">
            <input
              class="custom-radio"
              type="checkbox"
              id="radio-4"
              name="termsandcondition"
            />
            <label for="radio-4">
              <span class="dot"></span> You accepts our
              <a href="#">Terms and Conditions</a> and
              <a href="#">Privacy Policy</a>
            </label>
          </div>
        </div>
      </div>
      <div class="form-group row">
        <label class="col-md-3 col-form-label"></label>
        <div class="col-md-9">
          <button class="button">Post Your Job</button>
        </div>
      </div>
    </div>
  </form>
</template>

<script>
export default {
  name: "EmployerPostJob"
};
</script>

<style>
</style>