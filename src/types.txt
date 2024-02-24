#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
pub enum EditNoteStatus {
    Deleted,
    Edited,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
pub enum Fluency {
    Basic,
    Intermediate,
    Advanced,
    Native,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "oauth_code_challenge_method", rename_all = "lowercase")]
pub enum OauthCodeChallengeMethod {
    Plain,
    S256,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "taggable_entity_type", rename_all = "lowercase")]
pub enum TaggableEntityType {
    Area,
    Artist,
    Event,
    Instrument,
    Label,
    Place,
    Recording,
    Release,
    ReleaseGroup,
    Series,
    Work,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "ratable_entity_type", rename_all = "lowercase")]
pub enum RatableEntityType {
    Artist,
    Event,
    Label,
    Place,
    Recording,
    ReleaseGroup,
    Work,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "cover_art_presence", rename_all = "lowercase")]
pub enum CoverArtPresence {
    Absent,
    Present,
    Darkened,
}

#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "event_art_presence", rename_all = "lowercase")]
pub enum EventArtPresence {
    Absent,
    Present,
    Darkened,
}
// TODO: is this the right type?
#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "cube", rename_all = "lowercase")]
pub enum Cube {
    Cube,
}
// TODO is this the right type?
#[derive(Clone, Debug, PartialEq, PartialOrd, sqlx::Type)]
#[sqlx(type_name = "point", rename_all = "lowercase")]
pub enum Point {
    Point,
}
